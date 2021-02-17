# unitartu_tech_gazebo
Digital twin of UniTartuTech robotics lab. 

## How to setup
### Clone the repository in your catkin workspace. 
* https://github.com/ut-ims-robotics/unitartu_tech_gazebo.git

### Install dependencies
* Jackal
> * Simply use code below to install all jackal packages needed for the simulation to work. 
> * **sudo apt-get install ros-kinetic-jackal-simulator ros-kinetic-jackal-desktop ros-kinetic-jackal-navigation**
> * OR
> * https://github.com/jackal/jackal_simulator.git
> * https://github.com/jackal/jackal.git

* Universal robots
> https://github.com/ros-industrial/universal_robot.git
> 
### Build workspace
* *In your catkin workspace, run the following terminal commands;*
> * catkin_make
> * source devel/setup.bash
> 
### Launch 
* **Hallway(empty)**
  > roslaunch unitartu_tech_gazebo hallway.launch
* **Hallway(with jackal + doors)**
  > roslaunch unitartu_tech_gazebo hallway_jackal_doors.launch
* **Robotics room**
  > roslaunch unitartu_tech_gazebo ims_robotics.launch
