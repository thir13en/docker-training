# Commands


### docker run
For example, for running `redis`:
```shell
docker run redis
```

### docker version
List the version details

### docker ps
List running containers. can be run with `-a` to list all running and non running containers.

### Remove a container
	docker rm <container-id>

### List the images
	docker images

### Remove image
	docker rmi <img-name>

### Pull image but don't run container
	docker pull <img-name>