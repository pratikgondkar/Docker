# Problem Statement 
 Create a file named index.js with below content.
    index.js
    var os = require("os"); var hostname = os.hostname(); console.log("hello from " + hostname);
    Create a file named Dockerfile and write code as per the steps mentioned.
    Use alpine image.
    Add Author/Maintainer name in DockerFile
    run commands -> apk update & apk add nodejs
    copy current directory to /app
    change your working directory to /app
    specify the default command to be run upon container creation as mentioned below. node index.js
    Build image from Dockerfile.
    Tag image with name "hello:v0.1" 

Use all the best practices associated with Dockerfiles. Also, reduce the size of the image using multi-stage Dockerfile and other techniques.


-  Build the Docker Image
```
docker build -t hello:v0.1 .
```

- Run the Docker Container
```
docker run hello:v0.1

```
