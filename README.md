
#How to launch new navvis

```
roslaunch navvis navvis.launch bag_file:=/path/to/bag-file rviz_config_type:=no_track
```

rviz_config_type can be varied between no_track, track, no_map, and original. This new navvis launcher can launch the old robot and the new seamlessly.

#How to launch old navvis_description

To run the node with the default parameters, run the following.
```
roslaunch navvis_description navvis.launch
# OR, EXPLICITLY:
roslaunch navvis_description navvis.launch use_xacro:=true use_joint_state_publisher_gui:=true
```
To run the node with no GUI, run the following.

```
roslaunch navvis_description navvis.launch use_xacro:=true use_joint_state_publisher_gui:=false
```

The default use_xacro value has been changed to TRUE in the launch file navvis.launch.
