- Build the Docker Image
```
docker build -t yourname:docker-web .

```
- Run the Docker Container

```
docker run -d -p 8087:8080 yourname:docker-web

```

```
http://<virtualmachine_ipaddress>:8087/index.html

```

- Delete the Docker Container and Image
```
docker ps
docker stop <container_id>
docker rm <container_id>
docker rmi yourname:docker-web

```
