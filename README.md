# Setting up a graph node for existing ABI contracts

## Setup the graph node service
```
docker-compose up
```

## compile and setup the subgraph
```
yarn graph codegen
```
 ```
 yarn graph build
 ```

 ```
 yarn graph create --node http://localhost:8020 kalam360/subgraph-test
 ```

 ```
 graph deploy --node http://localhost:8020 --ipfs http://localhost:5001 kalam360/subgraph-test
 ```

## Setup the graph client

```
yarn graphclient build
```

```
yarn graphclient serve-dev
```