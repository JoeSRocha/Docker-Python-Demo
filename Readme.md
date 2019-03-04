

# What's Docker?
 - A tool to help you manage and scale your apps and its dependecies, easier.
 - Docker is an abstraction layer, sitting above the Host OS layer.
 - It leverages your native OS kernel, instead of running a "Guest OS" as you would on a Virtual Machine.
 - It is the encapsulation of an environment . Usually referenced as "Containerization".
![Docker](https://www.docker.com/sites/default/files/d8/styles/large/public/2018-11/container-what-is-container.png sf)

# Essentials: Images vs. Containers
- Docker Image: An inert, immutable file that's essentially a snapshot of a container.
- Docker Container: An image deployed on a Docker Engine.
- OOP Analogy: If a class is an image, then a Container is an instance of that class.

# Why would I need that?
 - Config once, run your app the same everywhere.
 - Faster than a VM workflow.
 - No more installing and managing app dependecies on your native OS.
 - Containers can deploy to [any server environment](https://aws.amazon.com/getting-started/tutorials/deploy-docker-containers/), including Production.
 - Leveraging Docker Config files, all environments will be kept in sync.


# Install Docker
https://www.docker.com/get-started
 - Disclaimer: Does not work on Windows Home Edition, but [Docker Toolbox](https://docs.docker.com/toolbox/toolbox_install_windows/) will.
 - Make sure to add your application path to Docker App Preferences, under `sharing`.
 - Recommended add-on: VSCode ext. Docker (Microsoft).
 - Other alternative GUIs exist as well, if you don't want to deal with CLI. [Kitematic](https://kitematic.com/), [DockStation](https://dockstation.io/)


# Hello Docker World
https://docs.docker.com/get-started/
```

# List all Docker images
$ docker image ls

# List all Docker Containers (--all shows stopped as well)
$ docker container ls --all
```

To create a Docker Image, all you need is a `Dockerfile` with the env. configuration.

```
# Create an Image, using the Dockerfile
$ docker build --tag=python-demo .

# Launch your Image as a container, binding local port 4000 to containers port 80
$ docker run -p 4000:80 python-demo
```

# Dockerhub
https://hub.docker.com/
- A cloud-based repository for the Docker community to build and distribute container images.
- Instead of building images, you can seek out official repos or take a chance with a random users  `repo`.
- You can also register on Docker Hub and upload and
