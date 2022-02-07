# Docker

## docker-compose
```
$ docker-compose build

$ docker-compose up
$ docker-compose -d

$ docker-compose ps

$ docker-compose stop <service-name>
```

## Use docker
[Link](https://qiita.com/jhorikawa_err/items/fb9c03c0982c29c5b6d5)  

Open Docker Desktop first.
```
$ docker image ls  # a list of available images

$ docker container ls  # running container

# If nothing shows up, go to the folder with `Dockerfile`
$ cd ~/Docker/py27
$ docker compose up -d --build  # make image -> launch container
$ docker compose up -d          # if the iamge is already built

# After you make sure the container is running
$ docker-compose exec python27 bash  # `python27` is the service name in `.yml`
```

## Python

Get packages info:
```
$ pip freeze > requirements.txt
```

## Unsolved error
```
py27jupyter  | Operation not permitted (src/thread.cpp:277)
py27jupyter  | qemu: uncaught target signal 6 (Aborted) - core dumped
```
Use Docker Desktop for Mac 4.0.1
