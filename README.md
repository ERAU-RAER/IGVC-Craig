# IGVC Craig

A collection of [ROS2](https://docs.ros.org/en/humble/index.html) packages that make up the autonomous vehicle Craig. This repo *could* be cloned directly into the source folder of a workspace to produce the full functionality of Craig.  
This repo also serves as a guide to developing and maintaining packages and working with ROS. This includes creating a workspace and packages, and best practices to developing a high-performance robot. Information about internal ROS functionality is still most available on official documentation: <https://docs.ros.org/en/humble/index.html>

## Craig Nodes

Remember: nodes are contained in packages, and a package can contain multiple nodes.
- [ ] Control Surface
- [ ] Hardware Interface
- [ ] Camera AI
- [ ] Mapping
- [ ] Pathfinding

## Linux usage:

source /opt/ros/humble/setup.bash
rqt is not an option in wsl!
ros2 run <package_name> <executable_name>

Package -> Executables -> Nodes

## ROS development
ROS is a framework that allows for parallel development of independent packages. ROS does _NOT_ contribute to the functionality of a project (With exception).  

## Workspace Structure
<img src="https://github.com/SrMeissel/RAER_Craig/assets/68983654/6b110de5-6fd3-44b6-9c88-09391d6919c1">

## C++ Package Structure
<img align=left src="https://github.com/SrMeissel/RAER_Craig/assets/68983654/ad104232-f573-4d4e-857c-c6478366186a">

## Python Package Structure
<img align=left src="https://github.com/SrMeissel/RAER_Craig/assets/68983654/3c8cca47-61ff-4c78-9505-030314ec1021">
