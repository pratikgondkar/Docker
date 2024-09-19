# Part 01
## Problem Statement 

Create a utility to host a static website via Docker with below features 

- The website should be accessed via your team domain name i.e
  - <name>.<team-name>.com
  - mohan.ntd.com
- The website should be up and running in below intervals
  - 10-12
  - 4-6
- Modify the utility so that in which first half it would be printing your name and in second half your buddy name. i.e below will be the output of curl command
  - 10-12 | Hello from Mohan
  - 4-6 | Hello from Pankaj


## Solution

- Build the Docker Image
```
docker build -t mohan-website .
```
- Run the Docker Container
```
docker run -d --name mohan-site -p 8087:80 mohan-website
```


# Part 02
## Problem Statement
Create a new container.

Create One directory Structure:

Data

 Ninjas

   Mohan
   Uma
   Shikha
   Mayank

Now make sure that if this container is getting run by Mohan then Mohan should be able to Write on Mohand Directory only and for others Mohan should only be able to read it.

## Solution 

```
docker build -t rana .

docker run -it --name rana rana /bin/bash

```
