# **teleop_twist_joy**

## **Goal:**
Translate Joystic input to command velocity to control robot motors 

## **Prerequisit **
Joy_node ros2
run it by
ros2 run joy joy_node


## **How it works:**
it recive standard /joy topic as input
in my case we use config/logitech.config.yaml to define what Joy axis and button are used as input

## **activate only the drive motors assuming**
ros2 launch launch/ros2_control_teleop-launch.py

## **Activate both Robot drive motors and whacker motor:**

Joy - Joystic node
joy_to_array_topic - used for generating /joint_whacker/command
ros2_control_teleop-launch.py - cmd_vel_joy generation

ros2 launch launch/joy-launch.py fron dev_ws


