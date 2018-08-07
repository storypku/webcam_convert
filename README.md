## How to use webcam on ROS Kinetic

### Prereq
- A notebook with Camera running Ubuntu 16.04
and ROS Kinetic

### Install usb-cam ROS package
```
sudo apt install ros-kinetic-usb-cam
```

### Download webcam_convert 
```
export CATKIN_WS=$HOME/devel/catkin_ws
cd $CATKIN_WS/src
git clone https://github.com/storypku/webcam_convert.git
```

### Build and Launch

```
cd $CATKIN_WS
catkin_make
source $CATKIN_WS/devel/setup.bash
roslaunch webcam_convert webcam_convert.launch
```
