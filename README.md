# opensim-containers
Containers for running OpenSim and utilities
Initially Docker containers based on Ubuntu 18.04 but will expand as needed. Layered as 
- opensim-deps (dependencies and build tools)
- opensim-pyhton (add in swig, python, build bindings)
- opensim-jave (add in swig, java, build bindings)
- opensim-core-cpp (core with no bindings)
- opensim-core-all (core with bindings)
- opensim-gui (add opensim-gui to opensim-java)

Possible directions to go:
- include open-pose
- include ML tools 
- include database layer, server, ...
