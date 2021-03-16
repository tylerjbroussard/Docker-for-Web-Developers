### https://docs.docker.com/engine/reference/commandline/docker/

**[ brackets ] strings without quotes for commands**

- docker pull [repo name]

  - pull images like hello-world

- docker images

  -will shows all docker image

- docker run [image name]

  - for running images in a container

- docker ps

  - lists all running containers

- docker ps -a

  - lists all containers on the system
  - you'll see container ID, alias (you can use instead of id) and status

- docker rm [container name]

  - removes a container, you can use the full string id or just a few characters
  - usually run this command then docker ps -a just the check, then you can clear the image if you need to...just for training

- docker rmi [image name]

  - this removes a image after you remove the container
  - you can use the id string or just a few characters
  - usually followed by docker images

after you pull the kitematic/hello-world-nginx images

- docker run -p 80:80 kitematic/hello-world-nginx

  - this means docker run port 80 forward to port 80 in container,
  - then followed by the image name, this runs a container with a server at an ip @ port 80

- docker stop [container id]

  - this will stop the container id you are running, you can use full or partial string
  - followed by docker ps or docker ps -a

There is a difference between containers and images, images needs running containers to be executed
