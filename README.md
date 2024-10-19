# javascript-calculator-precourse

## 문자열 덧셈 계산기

### 구현할 기능 목록

1. 조건에 따라 문자열 분리하기

- "//" 와 "\n" 가 있는 경우
  - 있다면, //"와 "\n" 사이에 위치하는 문자를 커스텀 구분자로 사용
  - 커스텀 구분자를 기준으로 문자열 분리
- "//" 와 "\n" 가 없는 경우
  - 쉼표(,)만 있는 경우
    - 쉼표(,)를 기준으로 문자열 분리
  - 세미콜론(;)만 있는 경우
    - 세미콜론(;)을 기준으로 문자열 분리
  - 쉼표(,)와 세미콜론(;)이 모두 있는 경우
    - 쉼표(,)와 세미콜론(;)을 기준으로 문자열 분리

2. 분리된 문자열에 한글 또는 알파벳이 있는지 확인한다.

- 숫자가 아닌 다른 값이 있는 경우 "[ERROR]"로 시작하는 메시지와 함께 Error를 발생시킨 후 애플리케이션은 종료

3. 분리된 문자열에서 공백(white space) 또는 빈 문자가 있는 경우 숫자 0으로 인식해 변경한다.
4. 분리된 문자열의 타입을 숫자 타입으로 변경한다.
5. 숫자 타입으로 변경한 숫자들의 합을 구한다.

### 예외 처리 목록

사용자의 입력이 아래의 조건에 하나라도 포함되는 경우 "[ERROR]"로 시작하는 메시지와 함께 Error를 발생시킨 후 애플리케이션은 종료

1. 쉼표(,) 세미콜론(;) "//"와 "\n" 외에 다른 특수 문자가 있는 경우
2. 한글 또는 알파벳이 있는 경우
3. 커스텀 구분자를 기준으로 삼았을 때, 커스텀 구분자 외 다른 특수 문자가 있는 경우
4. 분리된 문자열에 음수가 있는 경우
5. 커스텀 구분자가 여러개인 경우
