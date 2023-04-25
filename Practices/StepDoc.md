# Building an Ubuntu and Python Docker Image
*This section illustrates the building of a Docker image based on the latest version of Ubuntu.*
***

## Description of the files needed
To this end, two scripts are needed:
  - One is a bash script named `install_file.sh that does all the work on the Linux level.
  - Second one is `Dockerfile` which controls the building procedure for the image itself.
***

## Installation procedure
- we need to make sure `Docker` is installed.
- we need to have  `Dockerfile` and `install_file.sh` are in the same folder 
- Run the following command `docker build -t <your_docker_image_name:tag>` to build the Docker image. What comes after `:`is a tag you want to assign to your container.
- For e.g. docker build --tag python-docker
- Check if  image is now listed with: `docker images`.
- We can change tag also like this  docker tag python-docker:latest python-docker:v1.0.0
- Run the Docker container with `docker run <your_docker_image_name:tag>`.
- `docker ps` command will still show the running container.
- we can detach from a container by typing `Ctrl-P +Ctrl-Q`.
- Attaching to a Docker container is accomplished with the command `docker attach $CONTAINER_ID` (notice that a few letters of the $CONTAINER_ID are enough).
-  `exit` command stops the Docker container. It can be removed with `docker rm $CONTAINER_ID`.- 
- The Docker image can be removed via `docker rmi` if not needed any longer as this my take a considerable amount of space.

