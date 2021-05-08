## Creating First Docker image

```dockerfile
# Use an existing Docker image as a base
FROM alpine
# Download and install a dependency
RUN apk add --update redis
# Tell the image what to do when it starts as a container
CMD [ "redis-server" ]
```

### Build docker image from docker file 

​	`docker build .`

## Process:

<img src="/home/deepesh/Pictures/Screenshot from 2021-05-08 11-56-03.png"  />

## Tagging an image:

docker build -t [docker-id]/[name]:[version] .

`docker build -t dirus97/redis:latest .`

`docker build -t redis`

## Copy command inside dockerfile

<img src="/home/deepesh/Pictures/Screenshot from 2021-05-08 15-16-24.png" style="zoom:50%;" />

`COPY ./ ./`

## Port Mapping

<img src="/home/deepesh/Pictures/Screenshot from 2021-05-08 15-20-11.png" style="zoom: 50%;" />

`docker run -p 8080:8080 simpleweb`

## WORKDIR

<img src="/home/deepesh/Pictures/Screenshot from 2021-05-08 15-37-44.png" style="zoom:50%;" />

`WORKDIR /usr/app`

