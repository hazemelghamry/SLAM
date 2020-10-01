# SLAM
TO CREATE A WORKSPACE :
$ mkdir -p ~/catkinn_ws/src
$ cd ~/catkinn_ws/
$ catkinn_make
$ source devel/setup.bash
$ echo $ROS_PACKAGE_PATH
$ cd ..
$  echo "source ~/catkinn_ws/devel/setup.bash" >> ~/.bashrc
TO INSTALL THE PACKAGES :
$ cd ~/catkinn_ws/src
$ git clone https://github.com/hazemelghamry/SLAM.git
$ cd ..
$ catkin_make
