# docker
about docker

- build image
  - `$ docker build -t <name-of-your-docker-image> .`
    - `.` means location of all the single files of the current directory
- see image list
  - `$ docker image ls`
- create/run container
  - `$ docker run -d --name <name-of-your-docker-container> <name-of-your-docker-image>`
- bind mount
  - `-v` `<pathtofolderonlocation>`:`<pathtofolderoncontainer>`
