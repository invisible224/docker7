# Docker Commands for Containerization

This guide outlines basic Docker commands to manage containers and images.


# Check Docker version
docker --version

# Pull an image from Docker Hub
docker pull nginx

# List local images
docker images

# Run a container in detached mode, map host port 8080 to container port 80
docker run -d -p 8080:80 nginx

# List all running containers
docker ps

# List all containers (including stopped ones)
docker ps -a

# Stop a running container by container ID or name
docker stop <container_id_or_name>

# Remove a stopped container by container ID or name
docker rm <container_id_or_name>

# Remove a Docker image by image ID
docker rmi <image_id>

# Build a Docker image from a Dockerfile in the current directory
docker build -t my_custom_image .

# Log in to Docker Hub
docker login

# Tag and push the image to Docker Hub
docker tag my_custom_image <dockerhub_username>/my_custom_image
docker push <dockerhub_username>/my_custom_image
