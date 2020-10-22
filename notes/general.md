# General notes


### Definition
`Docker` is a set of `platform as a service` products that uses `OS-level virtualization` to deliver software in packages called `containers`.  
It is basically a `box` with an application and its related dependencies, libraries etc inside it.  
In docker we have those separate boundaries called `containers`. We place each service in one container with all the libraries and dependencies required for it. A `container` is a completely isolated environment with their own processes, network interfaces and their own mounts.

### Images
These are readymade templates of services like `MongoDb`, `NodeJs` etc, to run in containers. We can either use existing images from `docker.io` or create our own.  
Creating an Image of the service helps in shipping it for deployments. Then it is just running a simple command to get the server up and running.  