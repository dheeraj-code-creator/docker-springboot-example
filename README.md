
# command to run docker compose
docker-compose up --build -d

# steps to push docker-compose image to docker hub
docker images

# select image name and tag it to your docker hub repository name
docker tag docker-springboot-example:0.0.1-SNAPSHOT dheeraj1990kk/docker-springboot-example:0.0.1-SNAPSHOT

# push to docker hub
docker push dheeraj1990kk/docker-springboot-example

# Pull from docker hub to any machine
docker pull dheeraj1990kk/docker-springboot-example:0.0.1-SNAPSHOT

# run pulled images (Note for running docker-compose images command is different.)
docker-compose up -d

## if you will get any error then use below command to login your docker account and then follow below steps.
1. docker login --username=dheeraj1990kk
2. provide password
3. docker images
4. docker tag docker-springboot-example:0.0.1-SNAPSHOT dheeraj1990kk/docker-springboot-example:0.0.1-SNAPSHOT
5. docker push dheeraj1990kk/docker-springboot-example

# command to check containers
docker ps --all

# command to check images
docker images

# command to stop containers
docker stop container-id

# command to delete all containers
docker system prune

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

