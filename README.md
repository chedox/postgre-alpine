# postgre-alpine
Postgre docker image based on alpine linux

Installation
To use this image, you may choose one of these steps: build image from Dockerfile or pull docker image from docker hub.

Build image from Docker file First, clone Dockerfile from this github repository:

https://github.com/chedox/postgre-alpine

Then build the image by using this command:

docker build -t chedox/postgre-alpine:latest .

Pull docker image from docker hub (If you don't want to build the image manually)

docker pull chedox/postgre-alpine

To run this images, type this command:

docker run -d -p 27017:27017 -v ~/usr/apps/data/docker_data/postgredb:/data/db chedox/postgre-alpine:latest

Mounting volume
Data in container will be deleted automatically when you remove container. In order to keep your data from container although you had deleted your container, you need to mount your folder in your container to your local machine.

That's to put -v ~/usr/apps/docker_data/postgredb:/data/db

PostgreDB GUI interface
To use postgreDB GUI browser, you can use pgAdmin III.
