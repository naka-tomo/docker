# This is an auto generated Dockerfile for ros:ros-base
# generated from docker_images/create_ros_image.Dockerfile.em
FROM ros:noetic-ros-core-focal

# install bootstrap tools
RUN apt-get update && apt-get install --no-install-recommends -y \
    build-essential \
    python3-rosdep \
    python3-rosinstall \
    python3-vcstools \
    && rm -rf /var/lib/apt/lists/*

# bootstrap rosdep
RUN rosdep init && \
  rosdep update --rosdistro $ROS_DISTRO

# install ros packages
RUN apt-get update && apt-get install -y --no-install-recommends \
    ros-noetic-ros-base=1.5.0-1* \
    python3-catkin-tools \
    build-essential \
    && rm -rf /var/lib/apt/lists/* \
    && apt-get install  && apt-get install 

RUN echo "export PS1=\"${ROS_DISTRO} > \"" >> ~/.bashrc 
RUN ln -s /usr/bin/python3 /usr/bin/python
RUN echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
RUN echo "source /catkin_ws/devel/setup.bash" >> ~/.bashrc
RUN echo "export ROS_MASTER_URI=http://127.0.0.1:11311" >> ~/.bashrc
RUN echo "export ROS_HOSTNAME=127.0.0.1" >> ~/.bashrc
