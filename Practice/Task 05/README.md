## Command 
```
  docker run -it --name named-volume1 -v volume1:/opt:rw nginx bash
  docker volume ls
  docker volume inspect volume1 
  docker inspect named-volume1
  docker volume ls
  dcoker volume rm volume1
  docker volume rm volume1
  docker volume rm -f volume1
  docker rm -f $(docker ps -a)
  docker volume rm -f volume1
  dcoker volume ls
  docker volume ls
  docker volume prune
  docker volume ls
  docker volume --help
  docker run -d --mount type=tmpfs,destination=/app --name c1 nginx
  docker inspect c1
  docker run -d --name mysql -e MYSQL_ROOT_PASSWORD=password mysql
  docker volume ls
```
