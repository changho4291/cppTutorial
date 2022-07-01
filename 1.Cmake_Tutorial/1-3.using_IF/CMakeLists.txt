cmake_minimum_required( VERSION 3.16.3 )    # cmake 빌드 최소버전

# set 변수 생성
set(example_1 Hello)
set(example_2 "CMake!!")
set(example_3 30)
set(example_4 "30")

# 문자 변수값 - 결과 false
if(${example_1})
	message("true")
else()
	message("false")
endif()

# 문자 비교(STREQUAL) - 결과 true
if(${example_1} STREQUAL Hello)
	message("true")
else()
	message("false")
endif()

# 숫자 변수 값 - 결과 true
if(${example_3})
	message("true")
else()
	message("false")
endif()

# 숫자 변수 "값" - 결과 true
if(${example_4})
	message("true")
else()
	message("false")
endif()

# 숫자 비교(EQUAL) - 결과 false
if(${example_3} EQUAL 20)
	message("true")
else()
	message("false")
endif()