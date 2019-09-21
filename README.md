# mean-stack-docker
## MEAN Docker
App to show a Docker Compose set up for a mean application running Angular 7.

## Set up
Make sure you have docker and docker-compose installed.

Docker-compose should be version 1.6 or higher.

### Clone the repo
```bash
$ git clone https://github.com/radhouen/mean-stack-docker
```
 ### Run docker
 ```bash
 $ docker-compose up
 ```

 App should be running in `localhost:8181`





### commands

### container commads
sudo docker ps
docker container ls -a
docker container rm cc3f2ff51cab cd20b396a061
docker container ls -a --filter status=exited --filter status=created
docker container prune
docker container prune --filter "until=12h"
docker container stop $(docker container ls -aq)
docker stop angular-client

sudo docker system prune

sudo docker system prune --volumes

### images
docker image prune
docker image prune -a

## build Images
sudo docker build -t angular-client:dev .
## run container
sudo docker run -d --name angular-client -p 4200:4200 angular-client:dev


