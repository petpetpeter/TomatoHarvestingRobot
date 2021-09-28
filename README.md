# TomatoRoboto
A description for launching tomato robot in Hayashi's Lab

## Hardware List
- White Aleinware

## Tomato Detection


1. Launch RGB-D camera 
```
roslaunch realsense2_camera rs_rgbd.launch
```
2. Launch Tomato Detection (RGB-D in -> MarkerArray out)
```
rosrun tomato_detection handCameraYolor.py
```
3. Launch PLanner (MarkerArray in -> ClosetTomamto srv)
