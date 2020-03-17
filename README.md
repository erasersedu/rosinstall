# rosinstall

Ubuntu 16.04

*.Install git:

> sudo apt-get install git

*. Install wstool:

> sudo apt-get install python-wstool

#####
#####

1. Install ROS:

http://wiki.ros.org/kinetic/Installation/Ubuntu

#####
#####

2. Install Turtlebot

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


#####
#####

1. Install ROS in Ubuntu 18.04:

http://wiki.ros.org/melodic/Installation/Ubuntu


2. Install Turtlebot in Ubuntu 18.04:

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
2.2 Install Kobuki and Turtlebot:

(From: https://github.com/gaunthan/Turtlebot2-On-Melodic)


> cd ~/turtlebot_ws/src/

> bash ~/erasersedu_ws/rosinstall/src/ubuntu_18_turtlebot_basic.sh



3. Install OpenCV:

https://github.com/roboticslab-uc3m/installation-guides/blob/master/install-opencv.md


4. Install OpenNI/NITE:

https://github.com/roboticslab-uc3m/installation-guides/blob/master/install-openni-nite.md


5. Install OpenNI in ROS:

> sudo apt-get install ros-kinetic-openni*


