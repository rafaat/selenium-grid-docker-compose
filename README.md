#selenium-grid-docker-compose

**Requirements**
- docker
- docker-compose

**Start grid server**
- To start with single chrome and firefox node: `docker-compose up -d`
- To start with multiple nodes (for example 5 each): `docker-compose scale chrome=5 firefox=5`

**Check status of grid server**
- On MacOS: http://192.168.99.100:4444/grid/console
- On Linux: http://127.0.0.1:4444/grid/console

**Some useful docker commands**
- Check status of all images: `docker images -a`
- Check status of all containers: `docker ps -a`
- SSH into running container: `docker exec -it containerID bash`
- Force remove a container: `docker rm -f containerID`
- Force remove an image: `docker rmi -f imageID`
- Restart docker machine: `docker-machine restart default`
