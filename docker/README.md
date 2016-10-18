docker-hello-world
==================

**This image will be deprecated soon. Please use `dockercloud/hello-world` instead:**
https://hub.docker.com/r/dockercloud/hello-world/

Sample docker image to test docker deployments


Usage
-----

To create the image execute the following command on the docker-hello-world folder:

	docker build -t hello-world .


Running your Hello World docker image
-------------------------------------

Start your image:

	sudo docker run -d -p 80 hello-world

It will print the new container ID (like `d35bf1374e88`). Get the allocated external port:

	sudo docker port d35bf1374e88 80

It will print the allocated port (like 4751). Test your deployment:

	curl http://localhost:4751/


Hello world!

