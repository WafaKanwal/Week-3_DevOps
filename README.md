# Week-3_DevOps
docker build -t <image_name> .
Purpose: Builds a Docker image named <image_name> from the Dockerfile in the current directory.

docker run -d -p <host_port>:<container_port> <image_name>
Purpose: Starts a container from the <image_name> image, mapping <host_port> on the host to <container_port> in the container.

docker ps
Purpose: Lists currently running Docker containers.

docker ps -a
Purpose: Lists all Docker containers, including those that are stopped.

docker logs <container_id>
Purpose: Views the logs of the container with the specified <container_id>.

docker stop $(docker ps -q)
Purpose: Stops all running Docker containers.

docker rm $(docker ps -a -q)
Purpose: Removes all Docker containers, including those that are stopped.

docker rmi $(docker images -q)
Purpose: Deletes all Docker images.

docker volume rm $(docker volume ls -q)
Purpose: Removes all Docker volumes.

docker system prune
Purpose: Removes all unused Docker resources including stopped containers, unused networks, and dangling images.

docker exec -it <container_id> /bin/bash
Purpose: Opens an interactive bash shell inside the container with the specified <container_id>.

docker network ls
Purpose: Lists all Docker networks.

docker network inspect <network_name>
Purpose: Displays detailed information about the specified <network_name> network.

docker-compose up
Purpose: Starts up all services defined in a docker-compose.yml file.

docker-compose down
Purpose: Stops and removes all containers defined in a docker-compose.yml file.

docker-compose build
Purpose: Builds or rebuilds services defined in a docker-compose.yml file.

docker-compose logs
Purpose: Displays logs from all services defined in a docker-compose.yml file.

docker volume ls
Purpose: Lists all Docker volumes.

docker volume inspect <volume_name>
Purpose: Displays detailed information about the specified <volume_name> volume.

docker info
Purpose: Displays system-wide information about Docker.

docker tag <source_image> <target_image>
Purpose: Tags the <source_image> with a new name <target_image>.

docker push <image_name>
Purpose: Uploads the specified <image_name> to a Docker registry.

docker pull <image_name>
Purpose: Downloads the specified <image_name> from a Docker registry.

docker history <image_name>
Purpose: Shows the history of an image's layers.

docker save -o <file_name>.tar <image_name>
Purpose: Saves a Docker image as a tarball file <file_name>.tar.

docker load -i <file_name>.tar
Purpose: Loads a Docker image from a tarball file <file_name>.tar.

docker container prune
Purpose: Removes all stopped containers.

docker image prune
Purpose: Removes unused images.

docker network prune
Purpose: Removes all unused networks.

docker volume prune
Purpose: Removes all unused volumes.
