cmake_minimum_required( VERSION 3.16.3 )    # cmake 빌드 최소버전

# set 변수 생성
set(example_1 Hello)
set(example_2 "CMake!!")
set(example_3 30)
set(example_4 "30")

# 1. 문자 변수값 - 결과 false
if(${example_1})
	message("1. true")
else()
	message("1. false")
endif()

# 2. 문자 비교(STREQUAL) - 결과 true
if(${example_1} STREQUAL Hello)
	message("2. true")
else()
	message("2.false")
endif()

# 3. 숫자 변수 값 - 결과 true
if(${example_3})
	message("3. true")
else()
	message("3. false")
endif()

# 4. 숫자 변수 "값" - 결과 true
if(${example_4})
	message("4. true")
else()
	message("4. false")
endif()

# 5. 숫자 비교(EQUAL) - 결과 false
if(${example_3} EQUAL 20)
	message("5. true")
else()
	message("5. false")
endif()

# 6. SET 캐시
if(${cash1} EQUAL 20)
	message("6. true")
else()
	message("6. false")
endif()

# 7. SET STRING 캐시 1
if(${cash2} STREQUAL cmake)
	message("7. true")
else()
	message("7. false")
endif()

# 8. SET STRING 캐시 1
if(${cash3} STREQUAL "Hello Cmake")
	message("8. true")
else()
	message("8. false")
endif()