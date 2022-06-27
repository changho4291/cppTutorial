#  Hello Cmake!! 빌드 해보기
1. **cpp 프로젝트 만들기**</br>
	main.cpp 를 만들고 예제와 같이 코딩합니다.

2. **CMake 사용해보기**</br>
	프로젝트 폴더에 CMakeLists.txt 파일을 만들어 줍니다. CMake는 꼭 "CMakeLists.txt" 로 작성하셔야 합니다. 자세한 내용은 프로젝트를 참고하세요.

3. **빌드하기**</br>
	`$ mkdir build`</br>
	`$ cd build`</br>
	위와 같이 build 폴더를 만들어줍니다. build 폴더를 만드는 이유는 cmake 빌드 시 만들어질 목적파일들과 makefile 스크립트들이 프로젝트 내에 무질서하게 배치되는 것 을 막기 위함 입니다.</br>
	</br>
	`$ cmake ..`</br>
	터미널에 위와같이 명령을 입력해 cmake 빌드를 시작합니다. `..` 을 넣은 이유는 상위 폴더에 있는 "CMakeLists.txt" 를 찾기위함 입니다.</br>
	`$ make`</br>
	그 뒤 make 명령을 실행하여 최종 빌드를 하면 build 폴더 안에 프로젝트 명으로 바이너리 파일 하나가 만들어져 있을 것 입니다. 해당 예제에서는 Hello_Cmake 라는 이름으로 바이너리 파일이 있을 것 입니다.</br>
	`$ ./Hello_Cmake` 를 실행하여 정상적으로 컴파일이 완료 되었는지 확인합니다.

