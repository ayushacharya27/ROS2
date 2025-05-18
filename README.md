# ROS2 Installation is done

## After Installing we have to Source the our Terminal so that it knows where is ROS2 and where to run ROS2 from

```bash
source /opt/ros/humble/setup.bash
```
OR
```bash
. /opt/ros/humble/setup.bash
```

### This command makes the terminal know where to fetch ros2 from
If you type ros2 now the terminal will look for ros2 and if it finds it automatically appends the /opt/ros/humble/ in start 

### It also sets up the env variable to look to the correct version of ros

```bash
printenv | grep -i ROS
```

OUTPUT:

ROS1:
```bash
ROS_VERSION=1
PKG_CONFIG_PATH=/opt/ros/noetic/lib/pkgconfig:/opt/ros/noetic/lib/x86_64-linux-gnu/pkgconfig
ROS_PYTHON_VERSION=3
ROS_PACKAGE_PATH=/opt/ros/noetic/share
ROSLISP_PACKAGE_DIRECTORIES=
ROS_IP=127.0.0.1
ROS_ETC_DIR=/opt/ros/noetic/etc/ros
CMAKE_PREFIX_PATH=/opt/ros/noetic
PYTHONPATH=/opt/ros/noetic/lib/python3/dist-packages
ROS_MASTER_URI=http://localhost:11311
ROS_HOSTNAME=127.0.0.1
LD_LIBRARY_PATH=/opt/ros/noetic/lib:/opt/ros/noetic/lib/x86_64-linux-gnu
PATH=/home/ayush3112/.nvm/versions/node/v22.14.0/bin:/home/ayush3112/miniconda3/bin:/home/ayush3112/miniconda3/condabin:/opt/ros/noetic/bin:/home/ayush3112/.local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/home/ayush3112/unet-3.4.4/bin
ROS_ROOT=/opt/ros/noetic/share/ros
ROS_DISTRO=noetic
```

ROS2:
```bash
ROS_VERSION=2
ROS_PYTHON_VERSION=3
AMENT_PREFIX_PATH=/opt/ros/humble
PYTHONPATH=/opt/ros/humble/lib/python3.10/site-packages:/opt/ros/humble/local/lib/python3.10/dist-packages
LD_LIBRARY_PATH=/opt/ros/humble/opt/rviz_ogre_vendor/lib:/opt/ros/humble/lib/x86_64-linux-gnu:/opt/ros/humble/lib
ROS_LOCALHOST_ONLY=0
PATH=/opt/ros/humble/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
ROS_DISTRO=humble
```

## To make it permanent in order to run automiatically when u open a new terminal just paste it in the ~ /.bashrc

