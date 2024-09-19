## Command

```
2004  docker inspect c1
 2005  docker run -d --name c2 nginx
 2006  docker inspect c2 
 2007  docker network ls
 2008  docker run -d --name c3 nginx
 2009  dcoker inspect c3
 2010  docker inspect c3
 2011  docker rm -f $(docker ps -a)
 2012  docker run -d --name c1 nginx
 2013  docker run -d --name c2 nginx
 2014  docker inspect c1
 2015  docker inspect c2
 2016  docker exec -it c1 bash
 2017  docker exec -it c2 bash
 2018  docker inspect c1
 2019  docker inspect c2
 2020  docker network ls
 2021  docker network create custom
 2022  docker network ls
 2023  docker run -d --name c3 --network custom nginx
 2024  docker inspect c3
 2025  docker inspect custom
 2026  docker network ls
 2027  docker inspect bridge
 2028  docker inspect custom
 2029  docker exec -it c3 bash
 2030  docker network ls
 2031  docker network --help
 2032  docker network connect custom c2
 2033  docker inspect custom
 2034  docker inspect c2
 2035  docker exec -it c3 bash
 2036  docker exec -it c2 bash
 2037  docker network connect custom c1
 2038  docker inspect custom
 2039  docker exec -it c1 bash
 2040* 
 2041  docker exec -it c1 bash
 2042  docker run -d --name c4 nginx
 2043  docker inspect bridge
 2044  docker exec -it c1 bash
 2045  docker network connect custom c4
 2046  dcoker exec -it c4 bash
 2047  docker exec -it c4 bash
 2048  docker network ls
 2049  docker rm custom
 2050  docker network rm custom
 2051  docker network --help
 2052  docker netwok prune
 2053  docker network prune
 2054  docker network create new
 2055  docker network ls
 2056  docker network prune
 2057  docker network ls
 2058  docker network create new
 2059  docker network rm new
 2060  docker rm -f $(docker ps -a)
 2061  docker network ls
 2062  docker network rm custom
 2063  docker network ls
 2064  ifconfig
 2065  docker run -d --name host-container --network host nginx
 2066  docker inspect host-container
 2067  docker network inspect host 
 2068  docker ps
 2069  docker ps -a
 2070  docker logs -f d65a98cab861
 2071  docker run -d --name host-container --network host ubuntu
 2072  docker rm -f host-container
 2073  docker run -d --name host-container --network host ubuntu
 2074  docker ps
 2075  docker ps -a
 2076  docker logs -f 0726
 2077  docker logs -f 072642265d71
 2078  docker port 072642265d71
 2079  docker ps -a
 2080  netstat -tulnp
 2081  docker ps -a
 2082  hostname -i
 2083  docker rm -f host-container
 2084  docker run -it --name host-container --network host ubuntu bash
 2085  docker ps -a
 2086  docker ps
 2087  docker inspect host
 2088  docker inspect host-container
 2089  docker rm -f host-container
 2090  docker network ls
 2091  docker run -d --name none-container --network none nginx
 2092  docker ps
 2093  docker inspect none
 2094  docker exec -it none-container bash
```

```
docker network create --driver=bridge --subnet=192.168.0.0/16 network-name

docker network create --driver=bridge --subnet=172.28.0.0/16 --ip-range=172.28.5.0/24 --gateway=172.28.5.254 network-name

apt update -y && apt install iputils-ping -y
```
