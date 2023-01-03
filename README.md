# docker
about docker

- build image
  - `$ docker build -t <name-of-your-docker-image> .`
    - `.` means location of all the single files of the current directory
- see image list
  - `$ docker image ls`
- create/run container
  - `$ docker run -d --name <name-of-your-docker-container> <name-of-your-docker-image>`
- set port forwarding
  - `$ docker run -p <local-port>:<host-port> -d --name <name-of-your-docker-container> <name-of-your-docker-image>`
- sync with local folder
  - `$ docker run -v <pathtofolderonlocation>:<pathtofolderoncontainer> -p <local-port>:<host-port> -d --name <name-of-your-docker-container> <name-of-your-docker-image>`
- see list of docker container
  - `$ docker ps`
- bind mount
  - `-v <pathtofolderonlocation>:<pathtofolderoncontainer>`
