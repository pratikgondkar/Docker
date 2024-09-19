## Command
 
 ```
docker images
 2140  docker run -it --name c4 container-to-image bash
 2141  dcokerfile images
 2142  docker images
 2143  cat sudheer 
 2144  docker build -f sudheer -t new1 .
 2145  docker images
 2146  docker inspect new1
 2147  docker build -f sudheer -t new11 .
 2148  cat sudheer 
 2149  docker build -f sudheer -t new11 .
 2150  docker inspect new11
 2151  docker inspect new11 | grep ach
 2152  docker inspect new11 | grep Archtiecure
 2153  uname 
 2154  uname  -m
 2155  docker build -f sudheer -t new11 .
 2156  docker run -d --name c5 new11 echo sudheer
 2157  docker logs -f c5
 2158  docker build -f sudheer -t new11 .
 2159  docker run -d --name c6 new11 echo sudheer-append
 2160  docker logs -f c6
 2161  docker build -f sudheer -t new11 .
 2162  docker run -d --name c7 new11 
 2163  docker logs -f c7
 2164  docker build --build-arg VERSION=18.04 -t myimage .
 2165  docker run -it -e environment=production --name c8 myimage  bash
 2166  ls
 2167  cat sudheer 
 2168  docker build -f sudheer --build-arg VERSION=18.04 -t myimage .
 2169  docker run -it -e environment=production --name c9 myimage  bash
 2170  cat /etc/os-release 
 2171  docker ps
 2172  docker ps -a
 2173  docker rm -f $(docker ps -a)
 2174  cd
 2175  docker login -u pritam0517
 2176  docker imgaes
 2177  docker images
 2178  docker tag myimage pritam0517/myfirst-repository:latest
 2179  docker imgaes
 2180  docker images
 2181  docker push pritam0517/myfirst-repository
 2182  docker login -u pritam0517
 2183  docker image history
 2184  docker image ls
 2185  docker tag myimage pritam0517/private:latest
 2186  docker push pritam0517/private:latest
 2187  history
```
