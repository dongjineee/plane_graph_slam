
# Plane Graph

This repository contains the code for the Plane Graph optimize project using ROS and Gazebo.

## Setup

To get started, clone the repository and build the project using the following commands:

```
git clone https://github.com/dongjineee/plane_graph_slam.git
cd plane_graph_slam
catkin_make
```

## Setting

To get started, clone the repository and build the project using the following commands:

```bash
git clone https://github.com/dongjineee/plane_graph_slam.git
cd plane_graph_slam
catkin_make
```
## 1. RUN
```bash
rosrun qp_slam keyframe_node # keyframe node
rosrun qp_slam plane_frontend_node # plane frontend node
rosrun qp_slam backend_node # backend node
```

## 2. example environment using Gazebo
<p align = "center">
<img src="https://github.com/dongjineee/plane_graph_slam/assets/150753899/41c6cba6-1a39-47df-920f-ac39f5558641" width="600" height="400"/>
</p>

## 3. example result
<p align = "center">
<img src="https://github.com/dongjineee/plane_graph_slam/assets/150753899/336be401-1f1b-4710-b7a3-208b1bf3f76e" width="600" height="400"/>
</p>
<p align = "center">
<img src="https://github.com/dongjineee/plane_graph_slam/assets/150753899/b6a62d81-8663-44c2-a3c8-ffb766dc2646" width="600" height="400"/>
</p>


- Red points: Noise points
- Green points: Ground truth points
- Yellow points: Optimized points



## Project Tree

```bash
plane_graph_slam
├─ .gitignore
├─ CMakeLists.txt
├─ README.md
├─ include
│  └─ qp_slam
│     ├─ backend.h
│     ├─ keyframe.h
│     └─ tracker_cloud.h
├─ msg
│  ├─ key_m.msg
│  ├─ plane.msg
│  ├─ planes.msg
│  └─ pose.msg
├─ package.xml
└─ src
   ├─ backend.cpp
   ├─ front_plane.cpp
   └─ keyframe.cpp
```
