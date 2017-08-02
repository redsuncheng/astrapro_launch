# astrapro_launch
This is the ROS launch file for astrapro/LeTV camera, which can stream both Depth and color video simultaneously.

Usage:

Download Astra drivers from this link address

http://www.orbbec3d.net/Tools_SDK_OpenNI/2-Linux.zip

Unzip it and follow the readme instructions to install and test the sensor.

sudo apt-get install ros-kinetic-astra-camera

sudo apt-get install ros-kinetic-astra-launch

sudo apt-get install ros-kinetic-libuvc-camera

sudo chmod -R 777 /dev/bus/usb/001/064

Copy the Lepro_launch package into the catkin_ws/src directory, and goto
catkin_ws, run catkin_make, then launch the file using

roslaunch lepro_launch lepro.launch

Then both the depth and RGB are streaming.


