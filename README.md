# Nginx Demo


## hosts 

C:\Windows\System32\drivers\etc\hosts 
```
127.0.0.1 www.airchinacc.com
```


## build

```
docker build -t nginx-demo:v1 .
```


## run 

```
 docker  run -d --name nginx-demo1 -p 80:80 nginx-demo:v1
```

```
PS D:\work\front-demo\nginx-demo> docker ps
CONTAINER ID   IMAGE                                 COMMAND                  CREATED          STATUS          PORTS                NAMES
cfc51e1975bc   nginx-demo:v1                         "/docker-entrypoint.…"   37 seconds ago   Up 38 seconds   0.0.0.0:80->80/tcp   nginx-demo1
8ade2701ad5d   docker/dev-environments-go:stable-1   "sleep infinity"         5 hours ago      Up 5 hours                           cranky_murdock
```

## 交互式


```
docker exec -it nginx-demo1 /bin/bash
```
