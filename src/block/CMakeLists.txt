#SET(CMAKE_VERBOSE_MAKEFILE on)
#SET(CMAKE_CXX_COMPILER g++)
#SET(CMAKE_CXX_FLAGS_DEBUG "-O0 -Wall -g3")
#SET(CMAKE_CXX_FLAGS_RELEASE "-O3 -Wall")

#SET(CMAKE_BUILD_TYPE Debug)

#ADD_SUBDIRECTORY(util)
#ADD_SUBDIRECTORY(main)
#ADD_SUBDIRECTORY(net)
#ADD_SUBDIRECTORY(block)
AUX_SOURCE_DIRECTORY(${PROJECT_SOURCE_DIR}/common SRC_LIST)
AUX_SOURCE_DIRECTORY(${PROJECT_SOURCE_DIR}/common/net SRC_LIST)
AUX_SOURCE_DIRECTORY(${PROJECT_SOURCE_DIR}/common/thread SRC_LIST)
AUX_SOURCE_DIRECTORY(${PROJECT_SOURCE_DIR}/common/time SRC_LIST)
AUX_SOURCE_DIRECTORY(${PROJECT_SOURCE_DIR}/common/log SRC_LIST)

INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/common)
INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/common/net)
INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/common/thread)
INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/common/time)
INCLUDE_DIRECTORIES(${PROJECT_SOURCE_DIR}/common/log)

ADD_SUBDIRECTORY(serv)
ADD_SUBDIRECTORY(cli)

ADD_SUBDIRECTORY(serv-1)
ADD_SUBDIRECTORY(cli-1)
