#  Dockernize Symfony Flex Stack : Nginx, MariaDB, ES, MongoDB 


An environment based on docker and docker-compose to run Symfony Flex


## Setup

First, clone the repo

```bash
$ git clone @flex-docker flex
$ cd flex
```

## Setup

Start containers with docker-compose :

```bash
$ docker-compose up -d --build
```

Add www.app.local to the hosts file :

```bash
$ sudo vi /etc/hosts  # add 127.0.0.1 www.app.dev
```

SSH on aya_app container :

```bash
$ docker ps
$ docker exec -it [CONTANER_ID|CONTANER_NAME] /bin/bash  #aya_app
$ composer install
```

To stop all Docker containers:

```bash
$ docker stop $(docker ps -a -q)
```


## to be continued