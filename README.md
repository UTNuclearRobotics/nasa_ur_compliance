# nasa_ur_compliance
Custom launch and config files for UR compliance.

https://github.com/UTNuclearRobotics/nasa_ur_compliance

https://github.com/UTNuclearRobotics/ros_controllers/tree/kinetic-compliance/compliance_controller

### Installation:

git clone --recursive https://github.com/UTNuclearRobotics/nasa_ur_compliance

### Usage:

roslaunch nasa_ur_compliance ur5_ros_control.launch robot_ip:=192.168.1.102

roslaunch ur5_moveit_config ur5_moveit_planning_execution.launch

#### To toggle compliance ON/OFF:

rosservice call /compliance_controller/toggle_compliance "{}"

#### Other useful services:

rosservice call /wrench_to_joint_vel_pub/disable_compliance_dimensions

rosservice call /wrench_to_joint_vel_pub/adjust_stiffness

rosservice call /wrench_to_joint_vel_pub/adjust_damping
