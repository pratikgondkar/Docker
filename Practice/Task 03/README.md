## Command
```
docker run -d --name load-testing --memory=10m --memory-reservation=20m nginx
docker run -d --name load-testing --memory=10m  nginx
docker stats
yes > /dev/null &
docker run -d --name c7 --memory=20m --cpus=0.5 --memory-reservation=10m nginx
```
