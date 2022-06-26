cmake_minimum_required( VERSION 3.16.3 )    # cmake 빌드 최소버전

project(
	Hello_Cmake								# 프로젝트 명
	VERSION 0.1.0							# 프로젝트 버전
	DESCRIPTION "Hello Cmake!!"				# 프로젝트 설명
	LANGUAGES CXX_EXTENSIONS				# 프로젝트 사용 언어
)

add_executable(${PROJECT_NAME}				# 프로젝트 실행파일(빌드 타겟) 지정
	main.cpp
)