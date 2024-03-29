# General notes


### Definition
`Docker` is a set of `platform as a service` products that uses `OS-level virtualization` to deliver software in packages called `containers`.  
It is basically a `box` with an application and its related dependencies, libraries etc inside it.  
In docker we have those separate boundaries called `containers`. We place each service in one container with all the libraries and dependencies required for it. A `container` is a completely isolated environment with their own processes, network interfaces and their own mounts.

### More informal definition
It is a **container tecnology**

## Container
A stabdardized unit of software: a package of code and the dependencies and tooling needed for runnin it.

### Before Docker...
Developing complex systems was a very difficult process, given that many services had to share the same OS in a VM and developers usually runt on several compatibility issues. With Docker, we are able to deploy several `containers` in the same VM, each one with their **independent** `processes`, `networks` and `mounts`. This containers are a type of light virtualization, which means the containers share the same OS kernel. The type of containers docker uses are `LXE Linux Containers`, which are very difficult to set up and require messing up with low level access to the OS. Docker provides an abstraction above `LXE` containers that is user frien dly and easily accessible.

### Images
These are readymade templates of services like `MongoDb`, `NodeJs` etc, to run in containers. We can either use existing images from `docker.io` or create our own.  
Creating an Image of the service helps in shipping it for deployments. Then it is just running a simple command to get the server up and running.

### Containers vs VMs
* Every VM is a fully emulated computer which runs on an isolated environment. Contaienrs share system resources.
* VMs cause redundancy and performance overhead

### Docker Engine
Provides the virtualizatiin support on top of our OS to run multiple containers and grant them access to the resources of our OS. It is actually a virtual machine whose sole purpuse is to run docker container.

### Docker Desktop
Makes sure Docker Engine works and it ships a Deamon and a CLI, plus a UI.

### Docker Hub
Cloud of images to share Docker pieces.

### Docker Compose
Docker task runner.