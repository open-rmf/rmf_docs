.. _getting_started:

***************
Getting started
***************

Installation
============

Building `rmf_core` from source requires `gcc` version 8 or higher, or `clang` version 6 or higher.

::

   mkdir ws_rmf/src -p
   cd ws_rmf/src/
   git clone https://github.com/osrf/rmf_core.git
   cd ../
   source /opt/ros/eloquent/setup.bash
   rosdep update
   rosdep install --from-paths src --ignore-src -yr
   colcon build --cmake-args -DCMAKE_BUILD_TYPE=RELEASE


To manually override the compiler version, prefix the `colcon` command with the `CXX` parameter.

::

   sudo apt update && sudo apt install g++-8
   CXX=g++-8 colcon build --cmake-args -DCMAKE_BUILD_TYPE=RELEASE


Demonstrations
==============

`This repository <https://github.com/open-rmf/rmf_demos>`_ holds a number of demonstrations and examples of working with `rmf_core` and the other packages in the RMF ecosystem.
