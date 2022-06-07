Learning docker


What is docker ..?
Virtual machines vs containers
Architecture of docker
Installing docker
Development workflow



Docker is a platform for building, running and shipping applications.

Virtual machine is an isolated environment for running applications
While virtual machine is an abstraction of machine (virtual machine)


Installing docker

// check docs.docker.com

Docker development workflow


Dockerfile. File containing instruction to package our application into an image
Image contains everything the application needs to run. Example os, runtime environment eg:node , application files, third party libraries, environment variables etc.



Instruction on deploying application using docker

Start with os
Runtime environment ex node
Copy app files
Run entry file



Steps

Create a docker file called Dockerfile
From base image ex: linux or node: version
Tell docker to build our application using “docker build -t image-name reference to docker file” command  
To see all images run docker image ls command
Run your docker image with this command “docker run image-name”
Publish your docker image on docker hub with this command: “docker push username/docker-image”



Useful commands

// getting all running containers

Docker ps

// seeing even stopped containers

Docker ps -a

// running  a container in interactive mode

Docker run -it docker-image
