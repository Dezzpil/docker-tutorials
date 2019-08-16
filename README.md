# Learning Docker

## Tips and tricks

One liner to stop / remove all of Docker containers from [Coderwall](https://coderwall.com/p/ewk0mq/stop-remove-all-docker-containers)
```
docker stop $(docker ps -a -q)
docker rm $(docker ps -a -q)
```
