# More commands for Docker

## docker run <image>
runs a container with the image

## docker run -d <image>
leaves the terminal free for other work (detached mode) while running container

## docker run --name <container-name> <image>
runs a container with given name with the image

## docker run -p 8080:80 <image>
runs a container with given image and exposes 80 port of container to the 8080 port of host (host means mine)

## docker run -v $(pwd):/app <image>
runs a container with given image, mounts the directory (or path you give) as a volume to the directory after the colon

## docker run -it <image> sh
runs a container with given image, in interactive mode (shell to interact with container)

## docker ps
show all containers (running), to show all, add -a at end

## docker logs <container>
show logs of the container

## docker attach <container>
attach me to container to see inside container

## docker start <container>
start container

## docker stop <container>
stops container gracefully

## docker kill <container>
kills all containers (kind of like deleting)

## docker stop $(docker ps -q)
stops all running containers, -q gives ids

## docker rm <container>
remove container, add -f for forcefull

## docker <container> prune
removes all stopped containers

## docker cp <container>:/path/to/file ./
copies a file from path given from container to given directory (at end)
