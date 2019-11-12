# Docker Volumes

> A volume is a designated directory in a container, which is designed to persist data, independent of the container's life cycle

* Volume changes are excluded when updating an image
* Persist when a container is deleted
* Can be mapped to a host folder
* Can be shared between containers

### Mount a Volume

* Volumes are mounted when creating or executing a container
* Can be mapped to a host directory
* Volume paths specified must be absolute

Execute a new container and map the /data/src folder from the host into the /test/src folder in the container

```bash
$ docker run -i -t -v /data/src:/test/src nginx:alpine sh
```

* Create some files and see the changes in host operating system

### Use of volumes

* De-couple the data that is stored from the container which created the data
* Good for sharing data between containers
    * Can setup a data containers which has a volume you mount in other containers
* Mounting folders from the host is good for testing purposes but generally not recommended for production use
