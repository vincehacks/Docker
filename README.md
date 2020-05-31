# Docker

Created by Vince Chang </br>

Docker replace VMs. VMs will split up a server's resource to create multiple
"servers" using the same machine. Docker will virtualize the operating system!

#### CONTAINERS

- Docker will create containers that will replace VMs
- They are lightweight, isolated, and fast microcomputers
- You can have different versions of os
- It is fast because you only need one kernel, you can run centos, debian,
  ubuntu, byt all share the same linux kernel
- If were to us VMs, they have to have their own linux kernel

#### DOCKER HUB

- [Docker Hub](hub.docker.com)
- Images of what you can install from Docker Hub will be located here, the idea
  is to "pull" down the image from the hub
- Installing centos image:
- `docker pull centos`
- This will start up the container
- `docker run -d -t --name vincecontainer centos`

#### DOCKER COMMANDS

- Get inside a container
  - `docker exec -it vincecontainer bash`
- See how many containers are running
  - `docker ps`
- Stop a container
  - `docker stop containerName`
- Start a container
  - `docker start containerName`
- See the states of container
  - `docker stats`
