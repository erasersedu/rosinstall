# rosinstall

*.Install git:

> sudo apt-get install git

*. Install wstool:

> sudo apt-get install python-wstool

#####
#####

1. Install ROS:

Ubuntu 16.04:

http://wiki.ros.org/kinetic/Installation/Ubuntu

*

Ubuntu 18.04:

http://wiki.ros.org/melodic/Installation/Ubuntu

You might need to install the following individual packages:

> sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list

> sudo apt-key adv --keyserver hkp://ha.pool.sks-keyservers.net:80 --recv-key 421C365BD9FF1F717815A3895523BAEEB01FA116

> sudo apt update

Then

> sudo apt-get install ros-melodic-map-server

> sudo apt-get install ros-melodic-amcl

> sudo apt-get install ros-melodic-laptop-battery-monitor

> sudo apt-get install ros-melodic-move-base

> sudo apt-get install ros-melodic-navigation

> sudo apt-get install ros-melodic-yocs-*

#####
#####

3. Install OpenCV:

Ubuntu 16.04:

https://github.com/roboticslab-uc3m/installation-guides/blob/master/install-opencv.md

*

Ubuntu 18.04:

Install CUDA

https://www.pugetsystems.com/labs/hpc/How-to-install-CUDA-9-2-on-Ubuntu-18-04-1184/


https://www.pugetsystems.com/labs/hpc/How-To-Install-CUDA-10-together-with-9-2-on-Ubuntu-18-04-with-support-for-NVIDIA-20XX-Turing-GPUs-1236/


Install OpenCV

https://github.com/roboticslab-uc3m/installation-guides/blob/master/install-opencv.md

(Alternatively: https://demura.net/misc/16485.html )


4. Install OpenNI/NITE:

https://github.com/roboticslab-uc3m/installation-guides/blob/master/install-openni-nite.md


4.1 Install OpenNI in ROS:

Ubuntu 16.04:

> sudo apt-get install ros-kinetic-openni*


Ubuntu 18.04:

> sudo apt-get install ros-melodic-openni*
