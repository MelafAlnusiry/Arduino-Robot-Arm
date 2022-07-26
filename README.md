# Installing-Arduino-Robot-Arm

## Artificial intelligence task 🦾:<br />
**Installing the package arduino-robot-arm on ROS** <br />

### First thing we login to Ubuntu then open terminal and write those commands : <br />

`cd ~/catkin_ws/` <br />

`catkin_make` <br />

`cd ~/catkin_ws/src` <br />

`git clone https://github.com/smart-methods/arduino_robot_arm.git`  <br />

`cd ~/catkin_ws` <br />

`rosdep install --from-paths src --ignore-src -r -y` <br />

`sudo apt-get install ros-kinetic-moveit` <br />

`sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui` <br />

`sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher` <br />

`sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control` <br />

`sudo nano ~/.bashrc` <br />

at the end of the (bashrc) file add the follwing line <br />
`source /home/wesam/catkin_ws/devel/setup.bash` <br />
then ctrl + o <br />

`source ~/.bashrc`<br />

`roslaunch robot_arm_pkg check_motors.launch`

<br />

## Robot Arm View: 
<img src="images/RobotArm.png" width="500">

