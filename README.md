# Blog

# Installation Process

First check if you were added as a contributor

If yes:

```shell
git clone git@github.com:davidmkrtchyan991/blog.git
cd blog/
```

Rename the example file to `.env`
```shell
cp .env.example .env
```

Enter into `docker` folder
```shell
cd docker/
```

Run the docker containers using `docker-compose`

Note: check if you have docker and docker-compose install on your machine
```shell
docker-compose up -d
```

Note:For the first time it will take some time to download all images and create containers

Now you can check all running containers
```shell
docker-compose ps
```

Enter into `docker`
```shell
docker-compose exec --user=laradock workspace bash
```

Now you will have acces to `composer`
```shell
composer install
```
or
```shell
composer update
```

Go to the browser and navigate to `localhost`