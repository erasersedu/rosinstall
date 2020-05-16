# ROSINSTALL

A quick introduction to ROSINSTALL

# Prerequisites

What things you need to install the software and how to install them

```
You should have ROS installed.
You should have OpenCV and OpenNI installed.
You should have a working ROS workspace.
```

# Installation

## 0. Requirements

*.Install git:

```
sudo apt-get install git
```

*. Install wstool:

```
sudo apt-get install python-wstool
```

## 1. ROS Install:

### Ubuntu 16.04:

Follow the indications here:

```
http://wiki.ros.org/kinetic/Installation/Ubuntu
```

### Ubuntu 18.04:

First, follow the indications here:
```
http://wiki.ros.org/melodic/Installation/Ubuntu
```

Then, you might need to add the following repositories:

```
sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list
sudo apt-key adv --keyserver hkp://ha.pool.sks-keyservers.net:80 --recv-key 421C365BD9FF1F717815A3895523BAEEB01FA116
sudo apt update
```

Finally, install the necessary ROS packages:

```
sudo apt-get install ros-melodic-map-server
sudo apt-get install ros-melodic-amcl
sudo apt-get install ros-melodic-laptop-battery-monitor
sudo apt-get install ros-melodic-move-base
sudo apt-get install ros-melodic-navigation
sudo apt-get install ros-melodic-yocs-*
```

## 2. Install OpenCV:

### Ubuntu 16.04:

Follow the indications here:

```
https://github.com/roboticslab-uc3m/installation-guides/blob/master/install-opencv.md
```

### Ubuntu 18.04:

First, install CUDA 9 as described here:

```
https://www.pugetsystems.com/labs/hpc/How-to-install-CUDA-9-2-on-Ubuntu-18-04-1184/
```

Then, if your computer supports CUDA 10, follow these indications:

```
https://www.pugetsystems.com/labs/hpc/How-To-Install-CUDA-10-together-with-9-2-on-Ubuntu-18-04-with-support-for-NVIDIA-20XX-Turing-GPUs-1236/
```

Finally, install OpenCV as in here:

```
https://github.com/roboticslab-uc3m/installation-guides/blob/master/install-opencv.md
```

** Alternatively, you can follow these instructions:

```
https://demura.net/misc/16485.html
```

## 3. Install OpenNI/NITE:

Follow the instructions here (both Ubuntu 16.04 and 18.04):

```
https://github.com/roboticslab-uc3m/installation-guides/blob/master/install-openni-nite.md
```

### 3.1 Install OpenNI in ROS:

### Ubuntu 16.04:

Follow the indications here:

```
sudo apt-get install ros-kinetic-openni*
```

### Ubuntu 18.04:

Proceed as indicated in the following link:

```
sudo apt-get install ros-melodic-openni*
```
