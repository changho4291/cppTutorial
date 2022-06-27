cmake_minimum_required( VERSION 3.16.3 )    # cmake 빌드 최소버전

set(example_1 Hello)
set(example_2 CMake!!)

set(example_3 Hello CMake!!)
set(example_4 "Hello CMake!!")
set(example_5 ${example_1} ${example_2})
set(example_6 "${example_1} ${example_2}")

message(Hello CMake!!)
message("Hello CMake!!")
message(\n)
message(${example_1} ${example_2})
message("${example_1} ${example_2}")
message([[${example_1} ${example_2}]])
message(\n)
message(${example_3})
message(${example_4})
message(${example_5})
message(${example_6})

# set 과 if, function, message 를 활용한 예제를 만들어보자