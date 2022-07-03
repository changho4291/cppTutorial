# CMake if문 사용 해보기!!
1. **if문 사용해보기**</br>
	참고: https://cmake.org/cmake/help/latest/command/if.html, https://junstar92.tistory.com/209?category=980796</br>
	cmake에서 if문 사용 문법은 다른 프로그램 언어와 유사하게 if(조건) elseif(조건) else() 이 있다. 그러나 특이하게 endif() 라는 함수를 호출하여 if가 끝났다는 것 을 알려줘야 합니다.</br>
	조건 비교는 다른 언어처럼 '<, >, ==, ||, &&' 를 사용하지 않습니다.다. 대신 EQUAL, LESS, LESS_EQUAL, GREATER, GREATER_EQUAL, STREQUAL .... 를 대신 비교 연산자로 사용해야합니다. 자세한 설명은 위 참고를 확인하시면 좋습니다.

2. **set 응용 해보기**</br>
	참고: https://cmake.org/cmake/help/latest/command/set.html</br>
	예제 7, 8, 9 에는 정의 되어있지 않은 변수를 조건에 넣어 두었습니다.
	이를 초기화 해주기 위해서는 다음과 cmake 빌드 시 다음과 같이 옵션을 넣어 주셔야 합니다.
	***cmake -D 변수명=값***


3. **테스트**</br>

	`cmake -D cash1=20 -D cash2 = cmake -D "cash3:STRING=Hello Cmake" ..`