# ORB-SLAM2-application
#### ● Application and Installation, config files
#### ● Used Intel D435i - stereo setup
#### ● ORB-SLAM2 official [homepage](https://github.com/raulmur/ORB_SLAM2), ORB-SLAM2 ROS [homepage](https://github.com/appliedAI-Initiative/orb_slam_2_ros)
### ● Result [clip1](https://youtu.be/-jueoC-YqF4) : Stereo, 30fps, 1200 features

<br><br>

## Requirements and installation

### ● [IntelD435i setup and calibration](https://github.com/engcang/VINS-application/tree/Intel-D435i)
  + Used [Kalibr](https://github.com/ethz-asl/kalibr) as [here](https://github.com/engcang/vins-application#-calibration--kalibr---synchronization-time-offset-extrinsic-parameter) and referred [here](https://support.stereolabs.com/hc/en-us/articles/360012749113-How-can-I-use-Kalibr-with-the-ZED-Mini-camera-in-ROS-)

<br>

### ● Eigen3
  ~~~shell
   $ sudo apt install libeigen3-dev
   or
   $ wget -O eigen.zip http://bitbucket.org/eigen/eigen/get/3.3.7.zip #check version
   $ unzip eigen.zip
   $ mkdir eigen-build && cd eigen-build
   $ cmake ../eigen_source_folder_name && sudo make install
  ~~~

### ● Install ORB-SLAM2-ROS as [here](https://github.com/appliedAI-Initiative/orb_slam_2_ros)
 ~~~shell
  $ cd ~/catkin_ws/src && git clone https://github.com/appliedAI-Initiative/orb_slam_2_ros
  $ cd .. && rosdep install --from-paths src --ignore-src -r -y
  $ catkin build
 ~~~
