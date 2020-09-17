# Ariac-2019
This is the final solution of Ariac 2019 using Moveit. I would like to thanks Ishan patel and team whose solution was the reference for solving this problem.
Instructions for running package:
```
open four seperate terminals
source /opt/ros/melodic/setup.bash
source ~/catkin_ws/devel/setup.bash
roslaunch final_solution final_sol.launch


#Start moveit for arm1 (https://bitbucket.org/osrf/ariac/wiki/2019/tutorials/moveit_interface)
source ~/ariac_ws/install/setup.bash
roslaunch ur10_moveit_config move_group.launch arm_namespace:=/ariac/arm1

#Start moveit for arm2 (https://bitbucket.org/osrf/ariac/wiki/2019/tutorials/moveit_interface)
source ~/ariac_ws/install/setup.bash
roslaunch ur10_moveit_config move_group.launch arm_namespace:=/ariac/arm2

#Start node
rosrun final_solution main_node
