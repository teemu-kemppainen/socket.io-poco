cmake_minimum_required(VERSION 2.8.7)

project(socketiopoco)
set(CMAKE_BUILD_TYPE Release) # or Debug
add_subdirectory (src)

file(GLOB SIOPOCO_HEADERS "${CMAKE_CURRENT_SOURCE_DIR}/include/*.h")

INSTALL(FILES ${SIOPOCO_HEADERS}
  DESTINATION include/socketio-poco/)
