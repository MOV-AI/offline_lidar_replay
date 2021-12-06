# Offline Lidar replay

## Installation
```bash
mkdir -p catkin_ws/src && cd catkin_ws/src
git clone --recursive git@github.com:MOV-AI/offline_lidar_replay.git
cd catkin_ws && catkin build lidar_replay 
source devel/setup.bash
```
## Run
``` bash
roslaunch lidar_replay replay.launch
```
### Parameters

- rviz:= (true or false)
- lidar:= ("velodyne", "ouster" or "" for both))
- bagfile:= (path to the bagfile)

### Example
``` bash
roslaunch lidar_replay replay.launch rviz:=false lidar:="" bagfile:="~/lidar.bag"
```