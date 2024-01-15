# IGVC Craig

A collection of [ROS2](https://docs.ros.org/en/humble/index.html) packages that make up the autonomous vehicle Craig. This repo *could* be cloned directly into the source folder of a workspace to produce the full functionality of Craig. 
This repo also serves as a guide to developing and maintaining packages and working with ROS. This includes creating a workspace, packages, and best practices to developing a high-performance robot. This project uses the humble distrobution. Information about internal ROS functionality is still most available on official documentation: <https://docs.ros.org/en/humble/index.html>

### Craig's Nodes

> [!NOTE]
> Remember: nodes are contained in packages, and a package can contain multiple nodes.

- [ ] Control Surface
- [ ] Hardware Interface
- [ ] Camera AI
- [ ] Mapping
- [ ] Pathfinding

### Competition

Craig is being built to perform in the [Intellegent Ground Vehicle Competition](http://www.igvc.org/) starting 2024. The competition challanges collegiate teams to design a level 4 autonomous vehicle. The teams are judged on both the performance and design of the vehicle.

## ROS

ROS is a framework that allows for parallel development of independent packages. ROS does _NOT_ contribute to the functionality of a project (With exception). 
If you have not used ROS before you can install it [here](https://docs.ros.org/en/humble/Installation.html).

#### Frequently Forgotten Commands
 
- To run ROS CLI commands, you must source the setup file _For Every Terminal_: `source /opt/ros/humble/setup.bash`

- To run Packages, you must source their workspace _In a New Terminal_: `source install/local_setup.bash`

### Development Enviroment

#### WSL

Developing ros packages in Linux is usually the prefered option. However, running a virtual machine can often be unstable and limiting. Luckily an alternative is [Windows Subsystem for Linux](https://learn.microsoft.com/en-us/windows/wsl/about).  
WSL creates a linux terminal and filesystem within windows. It can be installed simply with:  
~~~
wsl --install -d <Distribution Name>
~~~
and launched the same way as any application.  

#### ROS Directory

The source code of any ROS project is stored within a [Package](https://docs.ros.org/en/humble/Tutorials/Beginner-Client-Libraries/Creating-Your-First-ROS2-Package.html). ROS is built so that you can seemlessly run any combination of packages at any time. Therefore each package contains it's own executables. To manage these executables and faciliate communication between them, Packages are stored in a [ROS Workspace](https://docs.ros.org/en/humble/Tutorials/Beginner-Client-Libraries/Creating-A-Workspace/Creating-A-Workspace.html).


### Workspace Structure
<img src="https://github.com/SrMeissel/RAER_Craig/assets/68983654/6b110de5-6fd3-44b6-9c88-09391d6919c1">

### C++ Package Structure
<img align=left src="https://github.com/SrMeissel/RAER_Craig/assets/68983654/ad104232-f573-4d4e-857c-c6478366186a">

### Python Package Structure
<img align=left src="https://github.com/SrMeissel/RAER_Craig/assets/68983654/3c8cca47-61ff-4c78-9505-030314ec1021">
