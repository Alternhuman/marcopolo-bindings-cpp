CMAKE_MINIMUM_REQUIRED(VERSION 2.6)

PROJECT(MARCOTEST)

SET( MARCOTEST_SRC
  ${CMAKE_SOURCE_DIR}/src/main.c
)

FIND_PACKAGE(MarcoCPPBinding)

ADD_EXECUTABLE(marcotest ${MARCOTEST_SRC})
TARGET_LINK_LIBRARIES(marcotest ${MARCOCPPBINDING_LIBRARY})