CMAKE_MINIMUM_REQUIRED( VERSION 2.8 )
PROJECT( readpic )

SET(CMAKE_CXX_COMPILER "g++")
SET( CMAKE_BUILD_TYPE Release )

SET(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
SET(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)

LINK_DIRECTORIES( ${PROJECT_SOURCE_DIR}/lib)
LINK_DIRECTORIES("/usr/lib")
INCLUDE_DIRECTORIES("/usr/include/ni")
INCLUDE_DIRECTORIES("/usr/include/openni2")

ADD_SUBDIRECTORY( ${PROJECT_SOURCE_DIR}/src )
