# icra_2020_ws
Demo materials for ICRA 2020 paper.

## Usage
This repository contains the state of catkin workspace of each robot in the demo. 
* ***master*** branch contains the common base code.
* ***jackal-ws*** branch contains Clearpath Jackal + Jetson TX2 workspace
* ***operator-ws*** branch contains packages necessary from the operator side 

``` bash
git clone -b <platform-branch> https://github.com/temoto-telerobotics-demos/icra_2020_ws
git submodule update --init --recursive
cd icra_2020_ws
```

If you want the latest versions of the submodules, then (after that the state of this workspace may not be the same as it was for the demo)
``` bash
git submodule foreach git pull origin master
```

Initialize the catkin workspace
``` bash
catkin_make
```

From now on use *catkin_make* or *catkin build*
