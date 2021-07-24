# General notes


### Definition
`Docker` is a set of `platform as a service` products that uses `OS-level virtualization` to deliver software in packages called `containers`.  
It is basically a `box` with an application and its related dependencies, libraries etc inside it.  
In docker we have those separate boundaries called `containers`. We place each service in one container with all the libraries and dependencies required for it. A `container` is a completely isolated environment with their own processes, network interfaces and their own mounts.

### Before Docker...
Developing complex systems was a very difficult process, given that many services had to share the same OS in a VM and developers usually runt on several compatibility issues. With Docker, we are able to deploy several `containers` in the same VM, each one with their **independent** `processes`, `networks` and `mounts`. This containers are a type of light virtualization, which means the containers share the same OS kernel. The type of containers docker uses are `LXE Linux Containers`, which are very difficult to set up and require messing up with low level access to the OS. Docker provides an abstraction above `LXE` containers that is user friendly and easily accessible.

### Images
These are readymade templates of services like `MongoDb`, `NodeJs` etc, to run in containers. We can either use existing images from `docker.io` or create our own.  
Creating an Image of the service helps in shipping it for deployments. Then it is just running a simple command to get the server up and running.  