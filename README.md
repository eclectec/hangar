## Run
```
docker compose up -d
```

## Test
http://localhost:8529

username: root

password: arango

## Dump Data
```
docker exec -it hangar arangodump --output-directory /dumps --server.database ${db-name} --server.password arango
```

## Load Data
```
docker exec -it hangar arangorestore --input-directory /dumps --server.database ${db-name} --server.password arango
```
