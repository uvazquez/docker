# Octoprint for Docker


`Still in active development. Have not tested this on the pi`


#### Quick Start:

* Lets start by building the image: `docker build -t octoprint:0.1 .`
* We should remove all the dangling images:  `docker image rmi $(docker images -q -f dangling=true)`. 
* Now lets create a container with the image we just created.
    > Create Container: `docker run -itd --name octoprint -p 5000:5000  octoprint:0.1 bash`