## 📁 구현 기능 목록

### 📍 게임 시작

- 게임 시작 문구 출력: `숫자 야구 게임을 시작합니다.`
- `Random.pickNumberInRange()`을 활용하여서 지정숫자 뽑는다.

### 📍 게임 진행

- 1에서 9까지 서로 다른 3자리의 수 입력 받는다
  - `Console.readLineAsync`을 활용하여서 입력 받는다.
- 조건에서 벗어나는 수 예외 처리: `[ERROR] 숫자가 잘못된 형식입니다.`
- 조건에 맞는 수 판별
  - 스트라이크 판별: 같은 수, 같은 자리인 경우
  - 볼 판별: 같은 수, 다른 자리인 경우
  - 낫싱 판별: 같은 수 전혀 없는 경우
- 결과 출력하기

  - `Console.print`을 활용하여서 출력한다.
  - 볼만 있는 경우: `N볼`
  - 스트라이크만 있는 경우: `M스트라이크`
  - 낫싱인 경우: `낫싱`
  - 볼과 스트라이크 둘 다 있는 경우: `N볼 M스트라이크`
  - 3스트라이크인 경우:

    `3스트라이크`

    `3개의 숫자를 모두 맞히셨습니다! 게임 종료`

    `게임을 새로 시작하려면 1, 종료하려면 2를 입력하세요.`

### 📍 게임 재시작 및 종료

- 게임 재시작: 1을 눌렀을 경우, 게임 진행 처음으로 돌아간다.
- 게임 종료: 2를 눌렀을 경우, 게임을 완전히 종료한다.