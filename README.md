# robot_arm_package

After install VirtualBox
              Ubuntu20.04
              ROS
              
Open terminal to make sure of ros installtion 
```
roscore
```
**The output**

![Screenshot from 2022-08-16 09-29-34](https://user-images.githubusercontent.com/108773322/184821160-bbe1ba6f-f94e-4b5b-8ee6-fe3f4b98d304.png)

Install catkin workspace or folder
```
mkdir -p ~/catkin_ws/src

cd ~/catkin_ws/

catkin_make
```

To be inside the src folder after creating catkin folder including src 
```
cd ~/catkin_ws/src
```

To get a spetial arm packages
```
git clone https://github.com/smart-methods/arduino_robot_arm.git 

cd ~/catkin_ws
```
rosdep install --from-paths src --ignore-src -r -y
```
  For noetic:::::::::::::::::
  ```
$ sudo apt-get install ros-noetic-moveit
$ sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
$ sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
$ sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control
```

```
sudo nano ~/.bashrc
```

at the end of the (bashrc) file add the follwing line
(source /home/wesam/catkin_ws/devel/setup.bash)
then 
ctrl + o
Enter
ctrl + x to exit and back

```
source ~/.bashrc
```
```
roslaunch robot_arm_pkg check_motors.launch
```

**The result:**

![Screenshot from 2022-08-16 09-04-11](https://user-images.githubusercontent.com/108773322/184821989-caacb29d-4d31-445a-a6bb-e965cb66860e.png)


