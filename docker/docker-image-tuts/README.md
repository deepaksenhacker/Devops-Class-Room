# docker-image-tuts

This document contains common Docker commands for working with the `docker-image-tuts` image and starting containers.

## Build image

```bash
docker build -t docker-image-tuts .
```

## List images

```bash
docker images
```

## Run container from image

```bash
docker run --name docker-image-tuts-container -d docker-image-tuts
```

If you want to run in interactive mode:

```bash
docker run --name docker-image-tuts-container -it docker-image-tuts /bin/bash
```

## Start and stop container

Start an existing container:

```bash
docker start docker-image-tuts-container
```

Stop a running container:

```bash
docker stop docker-image-tuts-container
```

Restart a container:

```bash
docker restart docker-image-tuts-container
```

## View running containers

```bash
docker ps
```

View all containers:

```bash
docker ps -a
```

## Logs and exec

View container logs:

```bash
docker logs docker-image-tuts-container
```

Execute a shell in a running container:

```bash
docker exec -it docker-image-tuts-container /bin/bash
```

## Cleanup

Remove stopped container:

```bash
docker rm docker-image-tuts-container
```

Remove image:

```bash
docker rmi docker-image-tuts
```
