## Making Directory Structure

```bash
mkdir ros2_ws
cd ros2_ws
mkdir src
```

## Now Since You made the directory now build it using colcon build

```bash
colcon build
```

## Now you will se files like
```bash
build  install  log  src
```

## Now source the install to setup.bash
```bash
. install/setup.bash
```

## Now to create Packages

### For C++ Uses Cmake.txt for c++ files

```bash
ros2 pkg create --build-type ament_cmake <package_name>
```

OR If you want with dependencies

```bash
ros2 pkg create --build-type ament_cmake <package_name> --dependencies rclcpp std_msgs
```

### For Python Uses setup.py for py files

```bash
ros2 pkg create --build-type ament_python <package_name> --dependencies rclpy std_msgs
```

# !!! Now for any changes , ANY CHANGES you make in the src file then try to colcon build again in the root directory

## Start Coding

### For Python save files in the src with the same name as package

### For cpp there will be another src files in the package





