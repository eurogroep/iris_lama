^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package iris_lama
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

1.4.0 (2024-03-11)
------------------
* Add an experimental lidar odometry. [Eurico Pedrosa]
* Build: install package.xml. [Rein Appeldoorn]
* Update build.yml. [Eurico F. Pedrosa]
* Add a simple pose graph optimizer. [Eurico F. Pedrosa]
* Fix ray computation. [Eurico F. Pedrosa]
* Node mask is now part of the container. [Eurico F. Pedrosa]
* Add ray casting computation with callback. [Eurico F. Pedrosa]

  By calling a user defined function for each cell the ray visits, we
  removed the need to store the visited cells before using them.
  This saves some cpu cyles and a memory.
* Fix build for melodic (#33) [Eurico F. Pedrosa]

1.3.1 (2022-09-02)
------------------
* Fix armhf compilation

1.3.0 (2022-09-01)
------------------
* Switch to plain cmake instead of a catkin based
* Several performance improvements
* Add a 2D slam solution based on pose graph optimization
* Add read support for more image types thanks to stb_image.h
* Add IO to the map data structure
* Introduce transient mapping to slam2d
* Reduce memory usage of the dynamic distance map by ~30%
* Fix a bug where some cells in the dynamic distance map were not update correctly

1.2.0 (2021-04-10)
------------------
* Expose localization covariance

1.1.0 (2020-12-05)
------------------
* Expose the global localization parameters as options
* Add option to mark free cells when there is no hit in SLAM (i.e. truncated ranges)
* Add non-motion update trigger to location
* Fix infinite loop in global localization
* Use C++14
* Fix eigen aligment issues

1.0.0 (2020-05-05)
------------------
* First official release.
