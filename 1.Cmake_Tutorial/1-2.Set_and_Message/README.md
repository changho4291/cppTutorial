# CMake set과 message 사용 해보기!!
1. **set 사용해보기**</br>
참고: https://cmake.org/cmake/help/latest/command/set.html</br>
	CMake에서 set은 변수를 생성하는 역할을 합니다. 프로그래밍으로 치면 `var demo = temp` 와 같은 역할로 생각하시면 됩니다.</br>
	set 사용은 다음과 같이 `set('변수명' "값")` 과 같은 포멧으로 작성합니다. 이렇게 생성된 변수는 `${변수명}` 과 같은 패턴으로 호출 가능합니다.</br>
	set은 옵션을 활용하면 캐시설정을 할수도, 환경변수 설정도 제어 가능합니다. set의 캐시를 활용하는 방법은 나중에 이어서 다루도록 하겠습니다.</br>
	더 자세한 내용은 위 참고의 링크를 확인해주세요.

2. **message 사용해보기**</br>
참고: https://cmake.org/cmake/help/latest/command/message.html</br>
	message 는 cmake 빌드시 로그를 출력하는 역할을 합니다. c언어로 치면 `printf("값");` 과 비슷한 역할을 한다고 볼 수 있습니다.</br>
	옵션에 따라 세부 동작이 달라지지만 옵션 없이 값을 작성한다면 cmake 빌드중에 작성한 message 가 출력됩니다.</br>
	사용은 다음과 같이 `message([옵션] "값")` 으로 맞춰 작성하면 됩니다.</br>
	더 자세한 내용은 위 참고 링크를 확인해주세요.

3. **테스트**</br>
	`$ cmake ..`</br>
	build 폴더 생성 후 위 명령을 입력하여 예제를 실행해봅시다.
	처음엔 빌드 로그에 project가 없다는 경고가 나오지만 그 뒤에 'Hello Cmake!!' 라는 문구가 출력됨을 볼 수 있을 것 입니다.
	자세한 동작 원리는 'CMakeLists.txt' 에 작성된 스크립트를 참고하시면 됩니다.
	
	