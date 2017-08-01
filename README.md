# mapping_environments
**Author:** [Federico Nardi](https://www.dis.uniroma1.it/~dottoratoii/students/306)


###Brief Description:###

This package contains Gazebo [world](http://gazebosim.org/tutorials?tut=build_world) files and ROS [launch](http://wiki.ros.org/roslaunch) files to setup a simulated environment for semantic mapping.


###Software compatibility:###

We have tested the package on **Ubuntu 16.04** with **ROS Kinetic** and **Gazebo 7.8**.


###Installation instructions:###

To use this package, first you need to setup a **ROS** workspace as explained in this [tutorial](http://wiki.ros.org/ROS/Tutorials/InstallingandConfiguringROSEnvironment).

Then, clone the repository and install it:

```
cd <HOME_FOLDER>
mkdir source
cd source
git clone https://github.com/schizzz8/mapping_environments.git
cd ~/catkin_ws/src
ln -s ~/source/mapping_environments .
cd ..
catkin_make
```


###Content###

The package presents the following directory structure:

1. `mehses`: where we store the 3D geometric models with textures of the simulated environments

2. `world`: where we store the *.world* files to open with **Gazebo**

3. `launch`: where we store the *.launch* files to setup the simulated environment for the experiments


###Getting Started###

As an example, you can quickly check the content of the `empty_world.launch` file to see how a simulation is started.

To test the package, run:

```
roslaunch mapping_environments turtlebot_my_mesh.launch
```
