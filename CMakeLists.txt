cmake_minimum_required(VERSION 2.8.3)
project(roslaunch_test_resolve_unless)
find_package(catkin REQUIRED)
catkin_package()

if (CATKIN_ENABLE_TESTING)
  find_package(roslaunch REQUIRED)
  roslaunch_add_file_check(tests/roslaunch_test.xml)
endif()
