

# What's Docker?
 - A tool to help you manage and scale your app and its dependecies, easier.
 - Docker is an abstraction layer, sitting above the Host OS layer.
 - It leverages your native OS kernel, instead of running a "Guest OS" as you would on a Virtual Machine.
 - It is "Containerization" of your environment dependencies.
![Docker](https://www.docker.com/sites/default/files/d8/styles/large/public/2018-11/container-what-is-container.png "Docker Graph")

# Why would I need that?
 - Config once, run your app the same everywhere.
 - Faster than a VM workflow.
 - No more installing and managing app dependecies on your native OS.
 - Containers can deploy to [any server environment](https://aws.amazon.com/getting-started/tutorials/deploy-docker-containers/), including Production.
 - Leveraging Docker Config files, all environments will be kept in sync.


# Install Docker
https://www.docker.com/get-started
 - Disclaimer: Does not work on Windows Home Edition, however [Docker Toolbox](https://docs.docker.com/toolbox/toolbox_install_windows/) will work.
 - Make sure to add your application path to Docker App Preferences, under `sharing`.
 - Recommended add-on: VSCode ext. Docker (Microsoft)


# Hello Docker World
https://docs.docker.com/get-started/
```

# Create an Image, using the Dockerfile
$ docker build --tag=python-demo .

// Launch your Image as a container, binding local port 4000 to containers port 80
$ docker run -p 4000:80 python-demo
```

# Docker Compose
