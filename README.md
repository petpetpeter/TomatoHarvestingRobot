# TomatoRoboto
A description for launching tomato robot in Hayashi's Lab

## Hardware List
- White Aleinware

## Tomato Detection

1. Launch RGB-D camera 
```
roslaunch realsense2_camera rs_rgbd.launch
```
or
```
roslaunch azure_kinect_ros_driver driver.launch
```
2. Launch Tomato Detection (RGB-D in -> MarkerArray out)
```
rosrun tomato_detection handCameraYolor.py
```
or
```
rosrun tomato_detection advanceBaseCameraYolor.py
```

## Xarm
```
roslaunch xarm7_moveit_config realMove_exec.launch
```
```
rosrun real_xarm advanceXarm.py
```
