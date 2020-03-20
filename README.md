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

2. Install Turtlebot

Ubuntu 16.04:

(From: http://www.programmersought.com/article/8124276168/)


> cd

> mkdir -p ~/erasersedu_ws/src/

> cd ~/erasersedu_ws

> catkin_make

*

> git clone https://github.com/erasersedu/rosinstall.git


#####
2.1 Install Rocon:

> sudo apt install pyqt5-dev-tools

*

> cd

> mkdir -p ~/turtlebot_ws/src/

> cd ~/turtlebot_ws

> catkin_make

*

> cd ~/turtlebot_ws/src/

> mkdir -p rocon

> cd rocon

> wstool init src -j5 ~/erasersedu_ws/rosinstall/src/rocon.rosinstall

> source /opt/ros/kinetic/setup.bash

> rosdep install --from-paths src -i -y

*

> cd ~/turtlebot_ws/

> catkin_make


#####
2.2 Install Kobuki:

> cd ~/turtlebot_ws/src/

> mkdir -p kobuki

> cd kobuki

*

> wstool init src -j5 ~/erasersedu_ws/rosinstall/src/kobuki.rosinstall

> source ~/turtlebot_ws/devel/setup.bash

> rosdep install --from-paths src -i -y

*

> cd ~/turtlebot_ws/

> catkin_make

#####
2.3 Install Turtlebot:

> sudo apt-get install ros-kinetic-rqt-robot-dashboard

> sudo apt-get install ros-kinetic-cmake-modules ros-kinetic-interactive-markers ros-kinetic-depth-image-proc ros-kinetic-xacro

*

> cd ~/turtlebot_ws/src/

> mkdir -p turtlebot

> cd turtlebot

*

> wstool init src -j5 ~/erasersedu_ws/rosinstall/src/turtlebot.rosinstall

> source ~/turtlebot_ws/devel/setup.bash

> rosdep install --from-paths src -i -y

*

> cd ~/turtlebot_ws/

> catkin_make


#####
2.4 Install ROS libraries:

> sudo apt-get install ros-kinetic-librealsense

> sudo apt-get install ros-kinetic-turtlebot

> sudo apt-get install ros-kinetic-turtlebot-apps

> sudo apt-get install ros-kinetic-turtlebot-interactions

> sudo apt-get install ros-kinetic-turtlebot-simulator

> sudo apt-get install ros-kinetic-ar-track-alvar-msgs

*

Ubuntu 18.04:

> cd

> mkdir -p ~/erasersedu_ws/src/

> cd ~/erasersedu_ws

> catkin_make

*

> git clone https://github.com/erasersedu/rosinstall.git


#####
2.1 Install Rocon:

> sudo apt-get install ros-melodic-rocon-*


#####
2.2 Install Kobuki and Turtlebot:

(From: https://github.com/gaunthan/Turtlebot2-On-Melodic)

> cd

> mkdir -p ~/turtlebot_ws/src/

> cd ~/turtlebot_ws/

> catkin_make

> sudo apt-get install ros-melodic-joy*

> bash ~/erasersedu_ws/rosinstall/src/ubuntu_18_turtlebot_basic.sh

> catkin_make


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


5. Install OpenNI in ROS:

Ubuntu 16.04:

> sudo apt-get install ros-kinetic-openni*


Ubuntu 18.04:

> sudo apt-get install ros-melodic-openni*
