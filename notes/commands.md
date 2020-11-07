# Commands


### docker run
For example, for running `redis`:
```shell
docker run redis
```

### List the version details
	docker version

### Relevant information on your docker install
	docker info

### List running containers. can be run with `-a` to list all running and non running containers.
	docker ps

### Remove a container
	docker rm <container-id>

### List the images
	docker images

### Remove image
	docker rmi <img-name>

### Pull image but don't run container
	docker pull <img-name>

### List all docker containers
	docker container ls -a

### Get details of a container
	docker inspect <container-name>

### Access logs of a certain container
	docker logs <container-name>