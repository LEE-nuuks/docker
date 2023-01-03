# docker
about docker

- build image
  - `$ docker build -t <name-of-your-docker-image> .`
    - `.` means location of all the single files of the current directory
- see image list
  - `$ docker image ls`
- remove image from image list
  - `$ docker image rm <id-of-your-image>`
- create/run container
  - without set up name of docker container 
    - `$ docker run -d <name-of-your-docker-image>`
  - with set up name of docker container
    - `$ docker run -d --name <name-of-your-docker-container> <name-of-your-docker-image>`
- set port forwarding
  - `$ docker run -p <local-port>:<host-port> -d --name <name-of-your-docker-container> <name-of-your-docker-image>`
- sync with local folder
  - bind mount
    - `$ ....-v <pathtofolderonlocation>:<pathtofolderoncontainer> ....`
  - `$ docker run -v <pathtofolderonlocation>:<pathtofolderoncontainer> -p <local-port>:<host-port> -d --name <name-of-your-docker-container> <name-of-your-docker-image>`
- see list of docker container
  - running container
    - `$ docker ps`
  - all container
    - `$ docker ps -a`
- remove or delete docker container from the container list
  - `$ docker rm <name-of-your-container> -f`


- sign in docker container shell
  - `$ docker exec -it <name-of-your-docker-container> bash`

