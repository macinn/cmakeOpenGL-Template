# CMakeList.txt : CMake project for cmakeOpenGL-Template, include source and define
# project specific logic here.
#

# Add source to this project's executable.
add_executable (cmakeOpenGL-Template "cmakeOpenGL-Template.cpp" "cmakeOpenGL-Template.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET cmakeOpenGL-Template PROPERTY CXX_STANDARD 20)
endif()

# TODO: Add tests and install targets if needed.
