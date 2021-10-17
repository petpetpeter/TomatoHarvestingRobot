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
rosrun tomato_detection baseCameraYolor.py
```
3. Launch PLanner (MarkerArray in -> ClosetTomamto srv)
```
rosrun tomato_detection poseTomatoPlanner.py
```

## Xarm
```
roslaunch xarm7_moveit_config realMove_exec.launch
```
```
rosrun real_xarm xarm7_tracIK.py
```
