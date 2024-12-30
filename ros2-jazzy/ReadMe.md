# Build
- `docker build ./ -t ros2_jazzy`

# Run
- `docker run -it -v $HOME/ros2_ws:/ros2_ws --net=host --name ros2_jazzy ros2_jazzy`

# Setup
```
cd /ros2_ws
mkdir src
colcon build
```