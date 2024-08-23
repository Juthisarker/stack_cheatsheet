# View all containers (including stopped ones)
docker ps -all

# Start a container by ID
docker start <container_id>

# Start a container and attach to it
docker start -a <container_id>

# Delete all containers, networks, images (not just dangling ones), and build cache
docker system prune

# Create a container using the busybox image
docker create busybox

# Run a container using the busybox image
docker run busybox

# View logs of a container by ID
docker logs <container_id>

# Create a container to ping google.com
docker create busybox ping google.com

# Start a container by ID
docker start <container_id>

# Stop a container by ID (waits 10 seconds before forcefully stopping)
docker stop <container_id>

# Kill a container by ID (immediately stops it)
docker kill <container_id>

# Execute a command inside a running container (e.g., access Redis CLI)
docker exec -it <container_id> redis-cli

# Run an interactive shell session in a busybox container
docker run -it busybox sh

# Build a Docker image from a Dockerfile in the current directory
docker build .
