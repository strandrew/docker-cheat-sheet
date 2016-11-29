# docker-cheat-sheet
## Images
### Build an image from Dockerfile
    $ docker build -t axux:12 .
### List images
    $ docker images
### Remove a created image
    $ docker rmi <id>

## Running images
### Starting a new container from an image
    $ docker run axux:latest
## Starting a new container from an image interactively
    $ docker run -it axux:latest /bin/bash
## Starting a new container and exposing published ports (and labeling the instance)
    $ docker run -it -P --name axux-test axux:latest  /bin/bash
## Restarting an existing container that has stopped
    $ docker start -i <image name>
    
## Ports
### Seeing exposed ports for a container
    $ docker port axux-test
