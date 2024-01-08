cmake_minimum_required (VERSION 2.6)
project (OXYGINE_FLOW)

# Set the C++ standard to C++20
set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

set(OXYGINE_FLOW_INCLUDE_DIRS ${CMAKE_CURRENT_SOURCE_DIR}/src)
add_library(oxygine-flow STATIC 
	src/flow/Scene.cpp 
	src/flow/Scene.h
	src/flow/flow.cpp 
	src/flow/flow.h
	src/flow/Transition.cpp 
	src/flow/Transition.h
)

set(OXYGINE_FLOW_INCLUDE_DIRS ${OXYGINE_FLOW_INCLUDE_DIRS} PARENT_SCOPE)
