# Docker build command with tag name
docker build -t dheeraj1990kk/docker-simple-example:latest .

# Docker run command
docker run -p 8086:8086 dheeraj1990kk/docker-simple-example

# Docker check all container
docker ps --all

#Docker stop command
docker stop container-id

# Docker delete container command
docker system prune

# command to run docker compose
docker-compose up --build -d

# command to check containers
docker ps --all

# command to check images
docker images

# command to stop containers
docker stop container-id

# command to delete all containers
docker system prune
