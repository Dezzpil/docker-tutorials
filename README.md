# Learning Docker

## Tips and tricks

One liner to stop / remove all of Docker containers from [Coderwall](https://coderwall.com/p/ewk0mq/stop-remove-all-docker-containers)
```
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
```

Can use filter:
```
docker rm $(docker ps -a -q -f status=exited)
```

Newer approach:
```
docker container prune --filter status=exited --force
```

To remove unused images:
```
docker rmi $(docker images -q -f dangling=true)
```
