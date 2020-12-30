# [Docker Tutorial](https://www.youtube.com/watch?v=3c-iBn73dDE&t=1s)

* What is Docker? 
* What is a Container technically?
* Docker vs. Virtual Machine
* Docker Installation
* Main Commands

| Command | Description |
| ------- | ----------- |
| `docker run <image_name>` | run the image, pulls it if not already pulled |
| `docker run <image_name>:version` | run the image with the given version, latest by default |
| `docker run -d <image_name>` | gives ID of the container, runs in detatched mode |
| `docker pull <image_name>` | pull the image from docker hub |
| `docker images` | all the existing images, `REPO`, `TAG`, `ID`, `CREATED`, `SIZE` |
| `docker ps` | list of only the running containers |
| `docker ps -a` | list of running & stopped containers |
| `docker ps --filter or -f "status=exited"` | list of only the stopped containers |
| `docker stop <id>`| stop the container with the ID(hash) |
| `docker start <id>` | start the stopped container with the ID(hash) |
| `docker run -p<host_port>:<image_port> redis` | port binding for running multiple images that have same ports |
| `docker run -p6001:6379 -d redis:4.0` | redis v4.0 running on port 6001 -d mode |
| `docker run -p6000:6379 -d redis` | another redis latest running on port 6000 -d mode |

* Debugging a Container
* Demo Project Overview - Docker in Practice
* Developing with Containers
* Docker Compose - Running multiple services
* Dockerfile - Building your own Docker Image
* Private Docker Repository
* Deploy our containerized application
* Docker Volumes - Persist data in Docker
* Volumes Demo - Configure persistence for our demo project