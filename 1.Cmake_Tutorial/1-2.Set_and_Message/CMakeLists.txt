cmake_minimum_required( VERSION 3.16.3 )    # cmake 빌드 최소버전

# set 변수 생성 기초 1
set(example_1 Hello)
set(example_2 CMake!!)

# set 변수 생성 기초 1
set(example_3 Hello CMake!!)
set(example_4 "Hello CMake!!")
set(example_5 ${example_1} ${example_2})
set(example_6 "${example_1} ${example_2}")

# message 출력 기초 1
message(Hello CMake!!)
message("Hello CMake!!")

message(\n)	# 줄바꿈

# message 출력 기초 2
message(${example_1} ${example_2})
message("${example_1} ${example_2}")
message([[${example_1} ${example_2}]])

message(\n)

# message 출력 기초 3
message(${example_3})
message(${example_4})
message(${example_5})
message(${example_6})