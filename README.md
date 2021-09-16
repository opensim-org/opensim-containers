OpenSim Containers
==================
Containers for running OpenSim and utilities.

Initially these are Docker containers based on Ubuntu 18.04 but the list can expand as needed. 
The files in this repo are not Docker images but rather scripts to build Docker images. Prebuilt images on dockerhub will be linked later.
To build an image from a file, use the command "docker build -f 'filename' ." from the folder of interest.

The containers are layered as follows
- opensim-deps (dependencies and build tools)
- opensim-pyhton (add in swig, python, build opensim-core python bindings)
- opensim-java (add in swig, java, build opensim-core java bindings)
- opensim-cpp (opensim-core with no bindings)
- opensim-gui (TODO add opensim-gui to opensim-java)

Possible directions to go:
- include open-pose
- include ML tools 
- include database layer, server, ...

Images created by the Dockerfiles in this repo are maintained on dockerhub under the stanfordnmbl organization
https://hub.docker.com/orgs/stanfordnmbl/repositories
The master branch will be for maintaining opensim-core latest environment but supported images are those for specific tags.
If you have ideas to imporove or slim down the images let us know by opening issues on this repo.

## Paths

OpenSim is installed to the environment variable `OPENSIM_INSTALL`. The dependencies are installed to `OPENSIM_DEPENDENCIES_HOME`.
 