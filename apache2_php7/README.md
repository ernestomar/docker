# Dockerfile for Apache 2 and PHP 7

In order to build this image:

`docker build .`

Create a new container

`docker run -d -p 80:80 --name my_container -v /path/to/my/local/src/folder:/var/www/html ID_OF_CONTAINER`