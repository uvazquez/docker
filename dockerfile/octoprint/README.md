# Octoprint for Docker

`Still in active development. Have not tested this on the pi`

#### Quick Start:

 - build form git: `docker build https://github.com/uvazquez/docker.git#master:/dockerfile/octoprint/dockerfile -t octoprint:latest`

* Remove all the dangling images:  `docker image rmi $(docker images -q -f dangling=true)`. 
* Create a container:  `docker run -itd -p 5000:5000 --privileged -v /dev:/dev octoprint:latest bash`

