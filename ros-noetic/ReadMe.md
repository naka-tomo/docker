# Build 
- `docker build ./ -t ros_noetic`

# Run
- `docker run -it -v $HOME/catkin_ws:/catkin_ws --net=host  --name ros_noetic ros_noetic`

# Setup
```
cd /catkin_ws
mkdir src
catkin_make
```
