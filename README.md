# Docker All Basic Commands

## These commands use case depends on our requirements.

#### Check docker version
`docker --version`
#### Check  available images
`docker images`
#### Check running containers
`docker ps`
#### Check all the containers running and stopped
`docker ps -a`
#### Pull docker image from docker hub
`docker pull <image_name>`
#### Run a container 
`docker run -d -p 8080:80 --name <container_name> <image_name> ` // -p define the host and conatiner ports 
#### Stop a running container
`docker stop <container_name OR ID>`
#### Remove Image
`docker rmi <image_name OR ID>`
#### Remove stopped container
`docker rm <container_name OR ID>`
#### Remove all the stopped containers
`docker comtainer prune`
#### Remove all the unused images
`docker image prune`
#### Build a docker image form Dockerfile
`docker built -t <image_name> <specify directory/ mostly used  . >`
#### Build and run all the containers and configurations from docker compose file
`docker-compose up -d`
// d is for detach mode
#### Stop all the containers and configurations from docker compose file
`docker-compose down`
#### Moving into running container
`docker exec -it <container_name OR ID> bash`
#### Check logs of running container
`docker logs <Container_name OR ID>`
#### Check Detailed info about docker container
`docker inspect <container_name OR ID>`
#### Push an image to docker hub 
`docker push <image_name>:<tag>`
#### Pause a container
`docker pause <container_name OR ID>`
#### Unpause a container
`docker unpause <container_name OR ID>`
#### Copy files between container and host
`docker cp <container_name>:<path_inside_container> <host_path>`
#### List all the docker networks
`docker network ls`
#### Detailed info about network
`docker network inspect <network_id>`
#### Create a new docker network
`docker network create <network_name>`
#### Remove unused Networks
`docker network prune`
#### List Docker Volumes
`docker volume ls`
#### Create Docker Volume
`docker volume create <volume_name>`
#### Remove all the unused Volumes
`docker volume prune`
#### Display the disk usage of images and containers
`docker system df`
#### View top processes within container
`docker top <container_name OR ID>`

