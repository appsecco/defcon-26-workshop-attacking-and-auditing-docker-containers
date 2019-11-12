# Docker run

### Running docker container

* Run the following command to start an ubuntu container

```bash
docker run ubuntu:latest echo "Welcome to Ubuntu"
```

![welcome ubuntu docker](images/docker-run-welcome-ubuntu.png)


* Run the following command to start an ubuntu container with interactive bash shell

```bash
docker run --name samplecontainer -it ubuntu:latest /bin/bash
```

![docker interactive bash](images/docker-interactive-bash.png)

### Find your containers

* Listing running containers

```bash
docker ps
```

![docker ps](images/docker-ps.png)

* Listing all containers (running/stopped)

```bash
docker ps -a
```

![docker ps -a](images/docker-ps-a.png)


### Listing docker images

```bash
docker images
```

![docker images](images/docker-images.png)


### Running container in detached Mode

* Run an alpine container in the background

```bash
docker run --name pingcontainer -d alpine:latest ping 127.0.0.1 -c 50
```

* Looking at the logs (stdout) of a container

```
docker logs -f pingcontainer
```

![docker detach logs](images/docker-detach-logs.png)

### Running nginx container and access the service

```bash
docker run -d --name nginxalpine -p 7777:80 nginx:alpine
```

* Accessing the container service from the host system using mapped port

```bash
curl localhost:7777
```

![accessing nginx from host](images/nginxalpine-host.png)

* Accessing the container service using the container IP and container port

```bash
docker exec -it nginxalpine sh

ip addr

curl 172.17.0.2:80
```

![accessing nginx from container port](images/nginxalpine-container.png)