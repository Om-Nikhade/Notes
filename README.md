Here are some of the most important and widely used Docker commands, essential for managing containers, images, volumes, and networks:

### 1. **Docker Images**
   - **`docker images`**: Lists all images on your local machine.
   - **`docker pull <image>`**: Pulls an image from a Docker registry (like Docker Hub).
   - **`docker rmi <image>`**: Removes an image from your local machine.
   - **`docker build -t <tag> .`**: Builds an image from a Dockerfile in the current directory with a specified tag.
   
### 2. **Docker Containers**
   - **`docker run <image>`**: Runs a container from a Docker image.
     - Common flags:
       - `-d`: Run container in detached mode (in the background).
       - `-p <host_port>:<container_port>`: Maps a container's port to the host.
       - `-v <host_dir>:<container_dir>`: Mounts a volume from the host to the container.
       - `--name <container_name>`: Assigns a name to the container.
   - **`docker ps`**: Lists running containers.
     - **`docker ps -a`**: Lists all containers (running and stopped).
   - **`docker exec -it <container> <command>`**: Runs a command inside a running container (e.g., bash for a shell).
   - **`docker stop <container>`**: Stops a running container.
   - **`docker start <container>`**: Starts a stopped container.
   - **`docker restart <container>`**: Restarts a container.
   - **`docker rm <container>`**: Removes a stopped container.
   - **`docker logs <container>`**: Displays the logs of a container.
   - **`docker inspect <container>`**: Retrieves detailed information about a container.
   - **`docker stats`**: Displays real-time resource usage statistics for running containers.
   - **`docker attach <container>`**: Attaches your terminal to a running container.
   
### 3. **Docker Volumes**
   - **`docker volume create <volume>`**: Creates a Docker volume.
   - **`docker volume ls`**: Lists all Docker volumes.
   - **`docker volume rm <volume>`**: Removes a Docker volume.
   - **`docker volume inspect <volume>`**: Displays detailed information about a volume.
   
### 4. **Docker Networks**
   - **`docker network ls`**: Lists all Docker networks.
   - **`docker network create <network>`**: Creates a new Docker network.
   - **`docker network rm <network>`**: Removes a Docker network.
   - **`docker network inspect <network>`**: Retrieves details about a Docker network.
   
### 5. **Docker Compose**
   - **`docker-compose up`**: Starts containers defined in a `docker-compose.yml` file.
   - **`docker-compose down`**: Stops and removes containers defined in a `docker-compose.yml` file.
   - **`docker-compose build`**: Builds Docker images defined in a `docker-compose.yml` file.
   - **`docker-compose logs`**: Displays logs from services defined in `docker-compose.yml`.

### 6. **Docker System Cleanup**
   - **`docker system df`**: Shows Docker disk usage.
   - **`docker system prune`**: Removes unused containers, networks, images, and optionally volumes.
   - **`docker image prune`**: Removes dangling images.
   - **`docker container prune`**: Removes all stopped containers.
   - **`docker volume prune`**: Removes all unused volumes.


