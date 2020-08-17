# udm_urdf

This package contains several urdf files as well as a launch file which allows viewing urdf files.

# Installation

To install this package you must clone it in the src folder of your catkin workspace(catkin_ws)

```sh
cd catkin_ws/src
git clone https://github.com/tarungoohuram/TP_TI_2_URDF
catkin build
cd ..
source devel/setup.bash
```

# Exexution

To view the urdf, after sourcing the setup.bash

```sh
roslaunch udm_urdf check_urdf.launch
```

By default, the box.urdf file will be displayed.

In the urdf folder of the package, there are box.urdf, cylinder.urdf, sphere.urdf, mesh.urdf and main.urdf

To display main.urdf, in a terminal type the following command:

```sh
roslaunch udm_urdf check_urdf.launch model:='$(find udm_urdf)/urdf/main.urdf'
```

Please note that single quotes are important.

