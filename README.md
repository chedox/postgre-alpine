# postgre-alpine

Postgre docker image based on alpine linux
-------------------------------------------

Installation
---------------
Clone Dockerfile from this github repository:

https://github.com/chedox/postgre-alpine


Then build the image by using this command:
--------------------------------------------

docker build -t chedox/postgre-alpine:latest .


To run this images, type this command:
---------------------------------------

docker run -v -v ~/usr/apps/data/docker_data/postgredb:/data/db -e POSTGRES_USER=test -e POSTGRES_PASSWORD=secret -d chedox/postgre-alpine:latest

Mounting volume
-----------------------

That's to put -v ~/usr/apps/docker_data/postgredb:/data/db

PostgreDB GUI interface
---------------------------
To use postgreDB GUI browser, you can use pgAdmin III or higher.
