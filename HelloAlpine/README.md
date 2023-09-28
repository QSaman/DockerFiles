# Running shell

## Using `docker compose`

```
docker compose up --build -d && docker compose exec alpine sh
docker compose down
``` 

# Using `docker`

```
docker run --name alpine -it alpine:latest /bin/sh
docker container rm alpine
```

