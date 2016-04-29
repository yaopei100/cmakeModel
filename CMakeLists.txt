#@brief  CMake config
#@author Yaopei
#@date   2015-07-22
#@note   This CMakeLists.txt for project CMakeModel

PROJECT(CMAKEMODE)
CMAKE_MINIMUM_REQUIRED(VERSION 2.4)

SET(CMakeModel_VERSION 1.0)

#set the whole include directory
INCLUDE_DIRECTORIES(
    ${PROJECT_SOURCE_DIR}/include
    /usr/local/include
    /usr/include
)

#set the whole lib directory
LINK_DIRECTORIES(
    ${PROJECT_SOURCE_DIR}/lib
    /usr/local/lib
)

#set exec file output directory
SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
SET(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)

#set sub directory
ADD_SUBDIRECTORY(src)
#ADD_SUBDIRECTORY(test)
