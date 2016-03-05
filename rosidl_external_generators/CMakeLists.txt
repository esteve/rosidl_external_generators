cmake_minimum_required(VERSION 2.8.3)

project(rosidl_external_generators NONE)

find_package(ament_cmake REQUIRED)

ament_export_dependencies(rosidl_cmake)

if(AMENT_ENABLE_TESTING)
  find_package(ament_lint_auto REQUIRED)
  ament_lint_auto_find_test_dependencies()
endif()

ament_package(
  CONFIG_EXTRAS "rosidl_external_generators-extras.cmake.in"
)
