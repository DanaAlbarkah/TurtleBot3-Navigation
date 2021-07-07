# TurtleBot3-Navigation  
1-open a new terminal
2- Launch Simulation World
 ```
$ export TURTLEBOT3_MODEL=burger
$ roslaunch turtlebot3_gazebo turtlebot3_world.launch

 ```
 3-open anthor terminal  
 4- Run Navigation Node  
  ```
$ export TURTLEBOT3_MODEL=burger
$ roslaunch turtlebot3_navigation turtlebot3_navigation.launch map_file:=$HOME/map.yaml

 ```
 5-Estimate Initial Pose by:
-Click the 2D Pose Estimate button in the RViz menu.  
-Click on the map where the actual robot is located and drag the large green arrow toward the direction where the robot is facing.  
-Repeat step 1 and 2 until the LDS sensor data is overlayed on the saved map.  
-Launch keyboard teleoperation node to precisely locate the robot on the map
-Move the robot back and forth a bit to collect the surrounding environment information and narrow down the estimated location of the TurtleBot3 on the map which is displayed with tiny green arrows.  

6-Set Navigation Goal by:  
-Click the 2D Nav Goal button in the RViz menu
-Click on the map to set the destination of the robot and drag the green arrow toward the direction where the robot will be facing.
This green arrow is a marker that can specify the destination of the robot.
The root of the arrow is x, y coordinate of the destination, and the angle θ is determined by the orientation of the arrow.
As soon as x, y, θ are set, TurtleBot3 will start moving to the destination immediately.



 
 
