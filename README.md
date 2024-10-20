# javascript-calculator-precourse

## 구현 기능 목록 
- [x] 문자열 입력 기능을 생성한다.  
 &emsp;   [x] "덧셈할 문자열을 입력해 주세요."를 콘솔에 출력한다.  
 &emsp;   [x] 제공된 라이브러리를 사용하여 콘솔에 사용자의 값을 입력받을 수 있도록 대기한다.  
 &emsp;   [x] 결과값을 저장할 변수를 선언한다. (기본값은 0으로 할당)
- [x] 구분자 판단하기  
 &emsp;   [x] 기본 구분자 변수 설정한다. - 쉼표(,) 또는 콜론(:)  
 &emsp;   [x] 입력받은 문자열이 "//"로 시작하는지 확인한다.  
 &emsp;   [x] 입력받은 문자열에 "\n"이 존재하는지 확인한다.  
 &emsp;   [x] "//"과 "\n" 사이의 구분자가 숫자가 아닌 문자인지 확인한다.  
 &emsp;     -> 숫자 혹은 문자열일 경우 `ERROR` 발생 후 애플리케이션을 종료 시킨다.  
 &emsp;   [x] 정상적인 구분자라면 구분자 변수에 재할당한다.
- [x] 커스텀 구분자 설정을 제외한 문자열에 구분자와 양수를 제외한 문자가 존재하는지 확인한다.   
-> 존재할 경우 `ERROR` 발생 후 애플리케이션을 종료 시킨다.  
- [x] 구분자를 이용하여 문자열에서 숫자 추출한다.
- [x] 추출된 숫자를 모두 더한다. - `결과값`
- [ ] 결과를 출력한다.  
 &emsp;   [ ] 제공된 라이브러리를 사용하여 콘솔에 `결과 : ${결과값}` 을 출력한다.   

**사용자값 입력 및 출력은 `@woowacourse/mission-utils` 라이브러리에서 제공하는 `Console` API를 사용하여 구현한다.**

### 예제로 확인한 특이사항
- 빈 문자열일 경우 0을 반환한다.
- 여러 구분자가 사용될 수 있다.
    - 커스텀 구분자 설정 시 기본 구분자를 포함하여 여러 구분자가 사용될 수 있다.(예상)

### `[ERROR]` 가 발생할 수 있는 경우  
- 숫자와 구분자를 제외한 다른 문자가 존재하는 경우 (커스텀 구분자 설정 형식 제외)
- 구분자가 문자가 아닌 숫자나 문자열일 경우
