# Autoware Manual Controller

Keyboard controller for Autoware.

# Build & Run

* Source ROS and Autoware.universe workspace first.

* Build the code

```shell
mkdir -p autoware_manual_control_ws/src
cd autoware_manual_control_ws/src
git clone https://github.com/evshary/autoware_manual_control.git
cd ..
colcon build
```

* Run

```shell
source install/local_setup.bash
ros2 run autoware_manual_control keyboard_control
```

# Usage

1. Toggle to external mode
2. Set GateMode to Drive
3. Adjust speed and steering angle
4. Enjoy driving :-)

```shell
------------------------------------
| Different Mode:                  |
|   z: Toggle auto & external mode |
|   x: GateMode => Drive           |
|   c: GateMode => Reverse         |
|   v: GateMode => Park            |
|   s: View current mode           |
| Speed:                           |
|   u: Increase speed              |
|   i: Set speed to 0              |
|   o: Decrease speed              |
| Steering Angle                   |
|   j: Left turn                   |
|   k: Set angle to 0              |
|   l: Right turn                  |
------------------------------------
```