# Docker Management

There are different commands which will be very handy while using and managing docker containers.

## Inspecting container or image

* Returns low-level information on Docker objects

```bash
docker inspect <container name>
docker inspect <image name>
```

* Let's inspect the `nginx:alpine` image

```bash
docker inspect nginx:alpine
```

![docker inspect nginx](images/docker-inspect-nginx.png)

## Docker history

* Show the history of an image

```
docker history jess/htop
```

![docker history](images/docker-history.png)

## Stopping and removing container

* Let's run a nginx container

```bash
docker run --name dummynginx -d nginx:alpine
```

* Identify the container name or id using `docker ps`

```bash
docker stop dummynginx
```

* To remove container, it has to be stopped. Then runt he below command

```bash
docker rm dummynginx
```

![docker stop and remove](images/docker-stop-and-remove.png)
