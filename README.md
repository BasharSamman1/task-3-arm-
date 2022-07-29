# task-3-arm-

after installing ROS successfully
next is installing the arm package.
Following the instruction in this link.

Starting from this step "mkdir -p ~/catkin_ws/src"
https://s-m.com.sa/ros.txt
and changing the version form kinetic to noetic 

also changing this step 
(source /home/wesam/catkin_ws/devel/setup.bash)

To

(source /home/Bashar/catkin_ws/devel/setup.bash)

----------------------------------------------------
The steps;
mkdir -p ~/catkin_ws/src

cd ~/catkin_ws/

catkin_make

cd ~/catkin_ws/src

git clone https://github.com/smart-methods/arduino_robot_arm.git 

cd ~/catkin_ws

rosdep install --from-paths src --ignore-src -r -y

sudo apt-get install ros-noetic-moveit

sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui

sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher

sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control

sudo nano ~/.bashrc

at the end of the (bashrc) file add the follwing line
(source /home/Bashar/catkin_ws/devel/setup.bash)
then 
ctrl + o

source ~/.bashrc

roslaunch robot_arm_pkg check_motors.launch



<img width="560" alt="rosTask3" src="https://user-images.githubusercontent.com/109452510/181825724-c2668c8a-8dc4-4290-8f2b-d80adbdf8e50.png">
<img width="545" alt="rosTask3 1" src="https://user-images.githubusercontent.com/109452510/181825735-070d04c0-6c55-49a0-bea8-de9af1f112b2.png">

