# Octoprint for Docker

`Still in active development. Have not tested this on the pi`

**Quick Start:**

- build image form git: `docker build https://github.com/uvazquez/docker.git#master:/dockerfile/octoprint/dockerfile -t octoprint:latest`
 - Remove all the dangling images:  `docker image rmi $(docker images -q -f dangling=true)`. 
 - Create a container:  `docker run --name octoprint -itd -p 5000:5000 --privileged -v /dev:/dev octoprint:test bash`

**Known errors**

 - > `Unexpected error while connecting to serial port: AUTO SerialException: '[Errno 13] could not open port /dev/ttyUSB0: [Errno 13] Permission denied: '/dev/ttyUSB0'' @ comm.py:_openSerial:2478 (hook default)`
