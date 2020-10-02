# SLAM
TO CREATE A WORKSPACE : <br/>
$ mkdir -p ~/catkinn_ws/src <br/>
$ cd ~/catkinn_ws/ <br/>
$ catkin_make <br/>
$ source devel/setup.bash <br/>
$ echo $ROS_PACKAGE_PATH <br/>
$ cd .. <br/>
$  echo "source ~/catkinn_ws/devel/setup.bash" >> ~/.bashrc <br/>
TO INSTALL THE PACKAGES : <br/>
$ cd ~/catkinn_ws/src <br/>
$ git clone https://github.com/hazemelghamry/SLAM.git <br/>
$ cd .. <br/>
$ catkin_make <br/>
TO LAUNCH THE FILE : <br/>
$ cd ~/catkinn_ws/ <br/>
$ roslaunch drone L1_start_simulation.launch <br/>
TO TAKE OFF : <br/>
rostopic pub /ardrone/takeoff std_msgs/Empty <br/>
TO CONTROL THE DRONE : <br/>
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
