cmake_minimum_required(VERSION 3.5)
project(twist_mux_msgs)

find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)


rosidl_generate_interfaces(${PROJECT_NAME}
  "action/JoyPriority.action"
  "action/JoyTurbo.action"
)

## EXPORTS
ament_package()
