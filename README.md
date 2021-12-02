# PhysioSense-ROS

## Overview

This is a ROS package that integrates data from multi-modal physiological sensors such as the Vicon Motion Capture, Xsens, Cometa EMG, Kistler force plates.
The package has been tested in ROS melodic and Ubuntu 18.04.

The library allows to combine a set of sensors for the analysis of the human state during various tasks to assess different factors such as ergonomics.

## Installation

This software is built on the Robotics Operating System [ROS](http://wiki.ros.org/ROS/Installation).

1. To install ROS Melodic follow the steps mentioned in the official website

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[http://wiki.ros.org/melodic/Installation/Ubuntu](http://wiki.ros.org/melodic/Installation/Ubuntu)


2. After installing ROS Melodic run the following commands to download this project.

```
source /opt/ros/melodic/setup.bash
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/src/
git clone https://github.com/rmm-VUB/physiosense-ros.git
cd ..
catkin_make
```

## Running instruction

To launch the launch file physiosense-ros node, run the following command.

```
cd ~/catkin_ws/
source devel/setup.bash
roslaunch physiosense-ros physiosense-ros.launch
```

## Description

### Vicon

The Vicon package is publishing data about the position of markers in 3D space tracked by the motion capture system. Other datas include measurements of devices connected to the Vicon lock, namely the [Cometa EMG](https://www.cometasystems.com/products/mini-wave-infinity) and the [Kistler plate 9260AA](https://www.kistler.com/en/product/type-9260aa/).

[Vicon installation instructions](/vicon/motion_capture/README.md)

### Xsens

The Xsens package publishes the output of the [MTw Awinda sensors](https://www.xsens.com/products/mtw-awinda). 

### Kistler

The Kistler package publishes the output of the [Kistler plate 9260AA](https://www.kistler.com/en/product/type-9260aa/).

## Publication







