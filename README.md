# Custom Husky

+ This pacakge uses the ROS2 Control plugin to control the robot. The parameters can be tuned in the file - `control.yaml` at `/custom_husky/config/control.yaml`

+ The URDF folder has a `custom_husky.urdf.xacro` file which need to be converted into `custom_husky.urdf` using the command:
```
$ ros2 run xacro -o custom_husky.urdf custom_husky.urdf.xacro
```
The robot_state_publisher used the static `.urdf` file instead of the `.urdf.xacro` one to publish the robot description on the `/robot_description` topic.