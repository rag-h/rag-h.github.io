## What is Docker?

### What happened before containers?

Developers would usually directly install all of the required dependencies onto their laptops. Depending on the OS being used by the developers the installations process would be different. Similarly, installation of all of these dependencies may require different steps and developers could run into different problems.

### What is a container?

It is a way to package an application with all the necessary dependencies and configurations. The package is also portable and it can be shared around. It makes development and deployment more efficient as everything is done on one isolated environment. A container is its own isolated development environment. The users do not need to install all the dependencies onto their OS directly as it is installed on the docker image. Users would just need to download the docker image and they would be able to use the dependencies. This makes setting up the development environment much easier. When deploying the image on a server, no environment configuration are needed on the server.

### Where do containers live?

The live in a container repository. Many companies have their own private repositories. There is also a public repository for docker containers.

### Technical Aspect of what a container is

- It consists of layers of images stacked on top of each other with its base usually being a linux image. This is useually alpine:3.10 due to its small size.The application image usually lies on the highest layer.
- Suppose i'm pulling the postgres:9.6 container. It will pull all the individual layers required as well. Suppose i then want to install the next version of postgres. Some of the individual layers that i need for it have already been downloaded. So it does not need to redownload the layers again.
- Docker Image: This is the actual package. The application packaged together with the required configurations and the dependencies. This is the artifact that is moveable.
- Docker Container: Actually starting the image now becomes a container.

### Docker vs Virtual Machine

- Operating systems have two layers, the kernal and the application layer. The applications run on the kernal layer.
- Docker virtualises the application layer. It uses the kernal of the host.
- Virtual machines have their own kernal layer and an application layer. It virtualises the complete operating system.
- The size of a docker image is smaller as they do come with a kernal layer.
-
