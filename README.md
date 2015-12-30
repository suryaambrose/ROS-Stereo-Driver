Dependencies
------------

* gstreamer-app-0.10: `sudo apt-get install libgstreamer-plugins-base0.10-dev`
* ROS: `sudo apt-get install ros-{indigo,jade}-desktop-full`

Setup
-----

1.  Install dependencies
2. Source your ROS distribution; e.g. `source /opt/ros/jade/setup.bash`
3. If you don't have a catkin workspace, create one; e.g. `WS=stereo-workspace && mkdir -p $WS/src && cd $WS/src && catkin_init_workspace`
3. `cd` into the `src` folder of your catkin workspace
4. Clone sources:
  * `git clone https://github.com/ros-drivers/gscam.git`
  * `git clone https://github.com/suryaambrose/ROSStereoDriver.git`
5. Go to the workspace root and build all packages: `cd .. && catkin_make`

Getting started
---------------

