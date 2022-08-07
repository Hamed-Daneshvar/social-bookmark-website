# Social Bookmark website
This is a social Bookmark website created with Django and allow you to bookmark any images on the web and share it with the other users.


## docker command for run Redis

### create a network for redis

```sh
docker network create -d bridge redisnet
```

### run the redis container

```sh
docker run -d -p 6379:6379  --name bookmark-redis --network redisnet redis:alpine
```

### use redis cli in your container

```sh
docker exec -it bookmark-redis redis-cli
```