# Docker

### How to Do a Clean Restart of a Docker Instance
```shell
# Stop the container(s) using the following command:
docker-compose down

# Delete all containers using the following command:
docker rm -f $(docker ps -a e-q)

# Delete all volumes using the following command:
docker volume rm $(docker volume ls -q)

# Restart the containers using the following command:
docker-compose up -d
```