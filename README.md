# unitartu_tech_gazebo
Digital twin of UniTartuTech robotics lab. 

 ***NB: ROS Melodic was used for development***

## **How to setup**
_______________________________________________
### Clone this repository in your catkin workspace 'src' folder. 
> * https://github.com/ut-ims-robotics/unitartu_tech_gazebo.git

### **Install all dependencies**
Clone the following packages to the 'src' folder.  
* TurtleBot3
> * https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git
* Jackal
> * https://github.com/jackal/jackal_simulator.git
> * https://github.com/jackal/jackal.git

* Universal robots
> https://github.com/ros-industrial/universal_robot.git

* Robotont
> * https://github.com/robotont/robotont_description.git
> * https://github.com/robotont/robotont_gazebo.git
> * https://github.com/robotont/robotont_nuc_description.git

> 
### **Build and source workspace**

* *In your catkin workspace, run the following terminal commands;*
> * catkin_make
> * source devel/setup.bash


## **Launch** 
---
After succesful setup, the digital twin can be launched. 

**Digital Twin with UR5 + Mobile robot**

*By default TurtleBot3 will be spawned. The current version works with only TurtleBot3. In future updates, it will be possible to define a specific robot to spawn in Gazebo.*
* roslaunch unitartu_tech_gazebo ur5+mobile.launch

**Robotics lab room with UR5**
* roslaunch unitartu_tech_gazebo ims_robotics.launch

**Digital Twin with Jackal**
* roslaunch unitartu_tech_gazebo jackal.launch

**Digital Twin with Robotont**
* roslaunch unitartu_tech_gazebo robotont.launch

**Digital Twin with TurtleBot3**
* roslaunch unitartu_tech_gazebo turtlebot.launch

**Digital Twin with UR5**
* roslaunch unitartu_tech_gazebo ur5.launch

**Empty Room + Hallway**
* roslaunch unitartu_tech_gazebo room+hallway.launch

---

## Controlling robots
It is possible to use moveit and teleop operations to control the robots in the digital twin. Detailed information can be found in the links below

Find information regarding controlling the UR5 robot here https://github.com/ros-industrial/universal_robot

Mobile robots teleop http://wiki.ros.org/teleop_twist_keyboard  