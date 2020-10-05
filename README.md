# SLAM
TO CREATE A WORKSPACE : <br/>
$ mkdir -p ~/catkin_ws/src <br/>
$ cd ~/catkin_ws/ <br/>
$ catkin_make <br/>
$ source devel/setup.bash <br/>
$ echo $ROS_PACKAGE_PATH <br/>
$ cd .. <br/>
$  echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc <br/>
TO INSTALL THE PACKAGES : <br/>
$ cd ~/catkin_ws/src <br/>
$ git clone https://github.com/hazemelghamry/SLAM.git <br/>
$ cd .. <br/>
$ catkin_make <br/>
TO LAUNCH THE FILE : <br/>
$ cd ~/catkinn_ws/ <br/>
$ roslaunch drone L1_start_simulation.launch <br/>
TO TAKE OFF : <br/>
$ rostopic pub /ardrone/takeoff std_msgs/Empty <br/>
TO CONTROL THE DRONE : <br/>
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
BUILDING RTAB_MAP :
$ sudo apt-get install ros-melodic-rtabmap ros-melodic-rtabmap-ros <br/>
$ sudo apt-get remove ros-melodic-rtabmap ros-melodic-rtabmap-ros <br/>
$ cd ~ <br/>
$ git clone https://github.com/introlab/rtabmap.git rtabmap <br/>
$ cd rtabmap/build <br/>
$ cmake ..  [<---double dots included] <br/>
$ make <br/>
$ sudo make install <br/>
$ cd ~/catkin_ws <br/>
$ git clone https://github.com/introlab/rtabmap_ros.git src/rtabmap_ros <br/>
$ catkin_make -j1 <br/>
