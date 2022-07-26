# Installing-Arduino-Robot-Arm

## About This Project <br />
The robot arm has 5 joints only 4 joints can be fully controlled via ROS and Rviz, the last joint **gripper** has a default motion executed from the Arduino code directly.<br />
<br />

## Breadboard View <br />
<img src="images/circuit.jpeg." width="500">
<br />

## Robot initial positions <br />
<img src="images/positions.jpeg." width="500">

## SetUp Arduino Robot Arm🦾:

**○ First thing we login to Ubuntu then open terminal and write those commands :**<br />

**○ Check the dependencies:**<br />
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

**○ Now update your `bashrc` script with the information about the new workspace:**<br />

`sudo nano ~/.bashrc` <br />

**○ at the end of the `bashrc` file add the follwing line** <br />
`source /home/wesam/catkin_ws/devel/setup.bash` <br />
**○ then ctrl + o**<br />

`source ~/.bashrc`<br />
**○ The final command to finally launch the Arm**<br />
`roslaunch robot_arm_pkg check_motors.launch` <br />

<br />

## ○ Robot Arm View🔎: 
<img src="images/RobotArm.png" width="500">

