cmake_minimum_required( VERSION 2.8 )
project(BackToTheCode)

include_directories(inc)

include_directories(/usr/local/cuda/samples/common/inc)

add_subdirectory(lib)

include_directories(lib/gmock/include lib/gmock/gtest/include tests/mocks)

add_subdirectory(src)

add_subdirectory(tests)
