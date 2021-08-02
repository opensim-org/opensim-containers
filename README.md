# opensim-containers
Containers for running OpenSim and utilities.

Initially these are Docker containers based on Ubuntu 18.04 but the list will expand as needed. 
The files in this repo are not Docker images but rather scripts to build Docker images. Prebuilt images on dockerhub will be linked later.
To build an image from a file, use the command "docker build -f 'filename' ." from the folder of interest.

The containers are layered as follows
- opensim-deps (dependencies and build tools)
- opensim-pyhton (add in swig, python, build opensim-core python bindings)
- opensim-java (add in swig, java, build opensim-core java bindings)
- opensim-core-cpp (core with no bindings)
- opensim-core-all (core with both python and java bindings)
- opensim-gui (add opensim-gui to opensim-java)

Possible directions to go:
- include open-pose
- include ML tools 
- include database layer, server, ...
