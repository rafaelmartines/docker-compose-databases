# Docker Compose Databases
I created this repository to easily have a docker-compose ready for each type of databases I use through my learning and career.

The databases you can find here are:
* [MongoDB](//www.mongodb.com)
* [MySQL](//www.mysql.com/)
* [Postgresql](//www.postgresql.org/)

## Setting up
On each folder you will find a file name .env.example create a new one by doing a copy and paste action or using a shell command like the Linux one right bellow:
```shell
cp .env.example .env
```
Change the database credentials and execute the command:
```shell
docker-compose up -d
```
> [!INFO]
> Just remember, for your applications have access to the database you can [include the docker containers on the same network](//docs.docker.com/engine/reference/commandline/network_connect/) or just put the IP of the host of the container, in this case, your PC to your database configuration files.

> [!WARNING]
> If you change the credentials on .env file and try to rebuild the docker, you need to remove the volume folders, since the credentials are store there after you build the docker image, if you don't remove, the new credentials will not be applied.
