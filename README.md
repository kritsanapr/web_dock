### How to run project with docker compose.

#### Setup

1. Build image with command `docker compose build`
2. Docker image with command `docker images` you will find image name in **web-dock-server**
3. If you want to know more about docker layer run `docker history web-dock-server`
4. Create a network with the same name in docker-compose.yml file with `docker network create web_network`
5. Check network with `docker network ls`
6. Run command `docker compose up -d` for start container.
7. Access container with `docker exec -it web_dock_server_1 sh`

#### Clear

1. Stop container with `docker compose down --rmi all` for stop container and remove simage that docker uses.
2. Remove volume with `docker volume rm web_dock_server_volume
3. Remove network `docker network rm web_network`

Docker space docker uses.
`docker system df`
