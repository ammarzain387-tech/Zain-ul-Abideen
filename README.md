# ROS 2 Obstacle Avoidance Robot

A simple ROS 2 Python node that controls a mobile robot using LiDAR data.

The robot moves forward when the path is clear. When it detects an obstacle, it turns toward the side with more free space.

## Features

- Reads LiDAR data from `/scan`
- Publishes movement commands to `/cmd_vel`
- Detects obstacles in front, left, and right
- Automatically turns away from obstacles
- Uses clear and readable Python code

## Requirements

- Ubuntu Linux
- ROS 2 Humble, Iron, or Jazzy
- Python 3
- A robot with:
  - LiDAR sensor
  - `/scan` topic
  - `/cmd_vel` velocity control
## ROS 2 Topics

### Subscribed topic

```text
/scan
