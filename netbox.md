from https://github.com/netbox-community/netbox-docker/wiki/Getting-Started

# clone
git clone -b release https://github.com/netbox-community/netbox-docker.git

# cd to dir
cd netbox-docker

# make override file
vi docker-compose.override.yml

version: '3.4'
services:
  nginx:
    ports:
    - 8000:8080

# pull image
docker-compose pull

# start
docker-compose up -d

# Stop all the containers
docker-compose stop

# bring it down and clean up/delete everything
docker-compose down -v