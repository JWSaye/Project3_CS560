# Project 3 ROS2 Notes


### TO INSTALL PACKAGE FOR ASSIGNMENT 

1. Set up environment variables for ROS.
<pre>
source /opt/ros/humble/setup.bash
</pre>
Also do any Windows or Mac specific setup

For example in Mac...
<pre>
export WEBOTS_HOME=/Applications/Webots.app
python3 local_simulation_server.py
</pre>

For example in windows...
<pre>
export WEBOTS_HOME=/mnt/c/Program\ Files/Webots
</pre>

2. Make the package
<pre>
cd Project3_CS560
colcon build
</pre>

3. Set up variables to use the package you just created
<pre>
source install/setup.bash
</pre>

### FOR SIMULATION USE
Start webots simulation with connect back to ROS in the virtual machine
<pre>
ros2 launch webots_ros2_homework4_python f24_robotics_2_launch.py
</pre>

### RUN CONTROLLER
In a new terminal, move into the f24_robotics directory and source the install script again.

Next, run the controller code:
<pre>
ros2 run webots_ros2_homework4_python webots_ros2_homework4_python
</pre>

### RUN Cartographer
In a new terminal, run the cartographer code:
<pre>
ros2 launch turtlebot3_cartographer cartographer.launch.py
</pre>
