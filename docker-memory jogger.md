### some commonly used Docker commands

1. ```docker version```: displays the current version of Docker installed on your system.
2. ```docker info```: displays detailed information about the Docker installation, such as the number of containers, images, and networks.
3. Dockerfile: text file that contains a series of instructions used to build a Docker image. 

  - ```FROM```: Sets the base image for the Docker image.
  - ```LABEL```: Adds metadata to the image.
  - ```WORKDIR```: Sets the working directory for the container.
  - ```ADD```: Copies files, directories, or remote URLs to the container.
  - ```COPY```: Copies files or directories to the container.
  - ```RUN```: Executes a command during the build process.
  - ```CMD```: Specifies the command to run when the container is started.  
  - ```ENTRYPOINT```: Specifies the executable to run when the container starts.
  - ```ARG```: Defines a build-time argument. 
  - ```EXPOSE```: Specifies the ports to be exposed by the container.
  - ```ENV```: Sets environment variables in the container.
  - ```VOLUME```: Specifies the volumes to be used by the container.
  -  ```USER```: Sets the user to run the container.
  - ```ONBUILD```: Specifies commands to be run when the image is used as a base image.

4. ```docker build -t <image name> .``` : builds a Docker image from a Dockerfile in the current directory and tags it with the specified image name.
5. ```docker images```: displays a list of all Docker images downloaded on your system.
6. ```docker run <image>```: runs a Docker container from a specified image.
7. ```docker run -p <host port>:<container port> <image>```: runs a container and maps the specified host port to the container port.
8. ```docker ps```: displays a list of all running Docker containers.
9. ```docker ps -a```: lists all the containers on your system, including running and stopped containers. 
10. ```docker stop <container ID>```: stops a running Docker container with the specified container ID.
11. ```docker rmi <image ID>```: removes the specified Docker image from your system.
12. ```docker logs <container ID>```: displays the logs for a specified container.
13. ```docker exec -it <container ID> bash```: opens a bash shell in a running container.
14. ```docker pull <image>```: downloads a Docker image from a registry.
15. ```docker tag <image> <new tag>```: This command creates a new tag for a Docker image.
16. ```docker push <image>```: pushes a Docker image to a registry.
17. ```docker inspect <container ID>```: displays detailed information about a specified container.
18. ```docker network ls```: displays a list of all Docker networks.
19. ```docker network create <network name>```: creates a new Docker network.
20. ```docker network connect <network name> <container ID>```: connects a container to a specified network.
21. ```docker network disconnect <network name> <container ID>```: disconnects a container from a specified network.
22. ```docker volume ls```: displays a list of all Docker volumes.
23. ```docker volume create <volume name>```: creates a new Docker volume.
24. ```docker system prune```: removes all stopped containers, dangling images, and unused networks and volumes.
25. ```docker container prune```: removes all stopped containers.
26. ```docker image prune```: removes all dangling images.
27. ```docker network prune```: removes all unused networks.
28. ```docker volume prune```: removes all unused volumes.
29. ```docker-compose up```: starts the Docker containers defined in the docker-compose.yml file.
30. ```docker-compose down```: stops and removes the Docker containers defined in the docker-compose.yml file.

#### Docker Swarm 
- ```docker info```: We can see whether Swarm is acive or not. By default it will be inactive.
- ```docker swarm init```: Initialize a Docker Swarm:.
- ```docker swarm join --token <token> <IP:port>```: Join a Docker Swarm as a worker.
- ```docker swarm join-token manager```: Docker swarm join-token manager.
- ```docker node ls```: List nodes in the Docker Swarm.
- ```docker service —help```: Service in swarm replaces docker run.
- ```docker service create --name <service_name> <image_name>```: Create a Docker service.
- ```docker service scale <service_name>=<replica_count>```: Scale a Docker service
- ```docker service ls```: List the services.
- ```docker service ps {service_name}```: To get more o/p.
- ```docker service update --image <new_image_name> <service_name>```: Update a Docker service.
- ```docker service rm <service_name>```:Remove a Docker service.
- ```docker service inspect <service_name>```: Inspect a Docker service.
- ```docker node update --availability drain <node_name>```: Drain a node in the Docker Swarm.
- ```docker swarm leave --force```: Remove a node from the Docker Swarm.
