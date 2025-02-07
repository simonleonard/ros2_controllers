## Build status

ROS2 Distro | Branch | Build status | Documentation | Released packages
:---------: | :----: | :----------: | :-----------: | :---------------:
**Rolling** | [`rolling`](https://github.com/ros-controls/ros2_controllers/tree/rolling) | [![Rolling Binary Build](https://github.com/ros-controls/ros2_controllers/actions/workflows/rolling-binary-build-main.yml/badge.svg?branch=master)](https://github.com/ros-controls/ros2_controllers/actions/workflows/rolling-binary-build-main.yml?branch=master) <br /> [![Rolling Binary Build](https://github.com/ros-controls/ros2_controllers/actions/workflows/rolling-binary-build-testing.yml/badge.svg?branch=master)](https://github.com/ros-controls/ros2_controllers/actions/workflows/rolling-binary-build-testing.yml?branch=master) <br /> [![Rolling Semi-Binary Build](https://github.com/ros-controls/ros2_controllers/actions/workflows/rolling-semi-binary-build-main.yml/badge.svg?branch=master)](https://github.com/ros-controls/ros2_controllers/actions/workflows/rolling-semi-binary-build-main.yml?branch=master) <br /> [![Rolling Semi-Binary Build](https://github.com/ros-controls/ros2_controllers/actions/workflows/rolling-semi-binary-build-testing.yml/badge.svg?branch=master)](https://github.com/ros-controls/ros2_controllers/actions/workflows/rolling-semi-binary-build-testing.yml?branch=master) <br /> [![Rolling Source Build](https://github.com/ros-controls/ros2_controllers/actions/workflows/rolling-source-build.yml/badge.svg?branch=master)](https://github.com/ros-controls/ros2_controllers/actions/workflows/rolling-source-build.yml?branch=master) |  | [ros2_controllers](https://index.ros.org/p/ros2_controllers/#rolling)
**Humble** | [`humble`](https://github.com/ros-controls/ros2_controllers/tree/humble) | [![Humble Binary Build](https://github.com/ros-controls/ros2_controllers/actions/workflows/humble-binary-build-main.yml/badge.svg?branch=master)](https://github.com/ros-controls/ros2_controllers/actions/workflows/humble-binary-build-main.yml?branch=master) <br /> [![Humble Binary Build](https://github.com/ros-controls/ros2_controllers/actions/workflows/humble-binary-build-testing.yml/badge.svg?branch=master)](https://github.com/ros-controls/ros2_controllers/actions/workflows/humble-binary-build-testing.yml?branch=master) <br /> [![Humble Semi-Binary Build](https://github.com/ros-controls/ros2_controllers/actions/workflows/humble-semi-binary-build-main.yml/badge.svg?branch=master)](https://github.com/ros-controls/ros2_controllers/actions/workflows/humble-semi-binary-build-main.yml?branch=master) <br /> [![Humble Semi-Binary Build](https://github.com/ros-controls/ros2_controllers/actions/workflows/humble-semi-binary-build-testing.yml/badge.svg?branch=master)](https://github.com/ros-controls/ros2_controllers/actions/workflows/humble-semi-binary-build-testing.yml?branch=master) <br /> [![Humble Source Build](https://github.com/ros-controls/ros2_controllers/actions/workflows/humble-source-build.yml/badge.svg?branch=master)](https://github.com/ros-controls/ros2_controllers/actions/workflows/humble-source-build.yml?branch=master) |  | [ros2_controllers](https://index.ros.org/p/ros2_controllers/#humble)


### Explanation of different build types

**NOTE**: There are three build stages checking current and future compatibility of the package.

1. Binary builds - against released packages (main and testing) in ROS distributions. Shows that direct local build is possible.

   Uses repos file: `$NAME$-not-released.<ros-distro>.repos`

1. Semi-binary builds - against released core ROS packages (main and testing), but the immediate dependencies are pulled from source.
   Shows that local build with dependencies is possible and if fails there we can expect that after the next package sync we will not be able to build.

   Uses repos file: `$NAME$.repos`

1. Source build - also core ROS packages are build from source. It shows potential issues in the mid future.
