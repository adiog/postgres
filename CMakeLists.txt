cmake_minimum_required(VERSION 3.4)
project(Postgres)

set(CMAKE_CXX_STANDARD 11)

INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR})
INCLUDE_DIRECTORIES(${CMAKE_CURRENT_SOURCE_DIR}/include)

FILE(GLOB_RECURSE SOURCE_FILES ${CMAKE_CURRENT_SOURCE_DIR}/src/lib/**.cpp)
ADD_LIBRARY(postgres ${SOURCE_FILES})
#TARGET_LINK_LIBRARIES(privacy_guard_unit_test PrivacyGuard gtest gmock pthread dl gpgme)
