# Build
- `docker build ./ -t ros2_humble`

# Run
- `docker run -it -v $HOME/ros2_ws:/ros2_ws --net=host --name ros2_humble ros2_humble`

# Setup
```
cd /ros2_ws
mkdir src
colcon build
```