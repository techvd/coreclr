cmake_minimum_required(VERSION 2.8.12.2)

set(CMAKE_INCLUDE_CURRENT_DIR ON)

set(SOURCES
  test6.c
)

add_executable(paltest_sscanf_test6
  ${SOURCES}
)

add_dependencies(paltest_sscanf_test6 CoreClrPal)

target_link_libraries(paltest_sscanf_test6
  pthread
  rt
  m
  CoreClrPal
)
