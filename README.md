# mycobot_ros

unofficial myCobot ROS Package

[![Image from Gyazo](https://i.gyazo.com/cb39b38ddfa678c58c538460fbaac1ef.jpg)](https://tiryoh.hateblo.jp/entry/2021/01/07/233848)

| | industrial_ci |
|:---:|:---:|
| main develop<br>([`main`](https://github.com/Tiryoh/mycobot_ros/tree/main)) | [![industrial_ci](https://github.com/Tiryoh/mycobot_ros/actions/workflows/industrialci.yml/badge.svg?branch=main)](https://github.com/Tiryoh/mycobot_ros/actions/workflows/industrialci.yml) |

* official repositories
    * https://github.com/elephantrobotics/myCobot
    * https://github.com/elephantrobotics/mycobot_ros
    * https://github.com/elephantrobotics/pymycobot

## Installation

### 1. Download this repository

```sh
cd ~/catkin_ws/src
git clone https://github.com/Tiryoh/mycobot_ros.git
```

### 2. Install the dependencies

```sh
rosdep install -r -y -i --from-paths .
```

### 3. Build the package

```sh
catkin build
catkin source # or "source ~/catkin_ws/devel/setup.bash"
```

Execute `download_gazebo_models.sh` to download the Gazebo models manually.

```sh
rosrun mycobot_gazebo download_gazebo_models.sh
```

## Usage
### Quick Launch

#### [MoveIt](http://moveit.ros.org/) + [Fake Controller](http://docs.ros.org/en/melodic/api/moveit_tutorials/html/doc/fake_controller_manager/fake_controller_manager_tutorial.html)

```
roslaunch mycobot_move_it_config demo.launch
```

![Screenshot from 2021-01-22 00-45-46](https://user-images.githubusercontent.com/3256629/105374594-3a93cf00-5c4b-11eb-89c7-fa4a10aed619.png)

#### [MoveIt](http://moveit.ros.org/) + [Gazebo](http://gazebosim.org/)

```
roslaunch mycobot_move_it_config demo_gazebo.launch
```

![Screenshot from 2021-01-22 09-52-26](https://user-images.githubusercontent.com/3256629/105430751-96844500-5c97-11eb-88fd-9fe772f98001.png)

## License

This repository is licensed under the MIT license, see [LICENSE](./LICENSE).  
Unless attributed otherwise, everything in this repository is licensed under the MIT license.

### Acknowledgements

* [elephantrobotics/myCobotROS](https://github.com/elephantrobotics/myCobotROS)
    * `Copyright (c) 2020, Elephant Robotics`
    * [BSD-2-Clause](https://github.com/elephantrobotics/myCobotROS/blob/cc9c7151b60709c445e1d2bdf500b9fbad91f841/LICENSE)
* [rt-net/jnmouse_sim](https://github.com/rt-net/jnmouse_sim)
    * `(C) 2020 RT Corporation <support@rt-net.jp>`
    * [Apache-2.0](https://github.com/rt-net/jnmouse_sim/blob/5b3eac2071e7feb7e9ffd6f054cdfef9081e9166/LICENSE)
* [ros-planning/moveit](https://github.com/ros-planning/moveit)
    * `Copyright (c) 2008-2013, Willow Garage, Inc.`
    * [BSD-3-Clause](https://github.com/ros-planning/moveit/blob/664ae01803abf5e0b4649063102357262de9e05c/LICENSE.txt)

#### License Notice for Apache License, Version 2.0 Derivative Works

This software includes works that is distributed in the Apache License 2.0.  
https://www.apache.org/licenses/LICENSE-2.0