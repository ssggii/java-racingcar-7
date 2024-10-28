# java-racingcar-precourse

## 기능 요구사항
- [x]  주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
- [x]  각 자동차에 이름을 부여할 수 있다. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
- [x]  자동차 이름은 쉼표(,)를 기준으로 구분하며 이름은 5자 이하만 가능하다.
- [x]  사용자는 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
- [x]  전진하는 조건은 0에서 9 사이에서 무작위 값을 구한 후 무작위 값이 4 이상일 경우이다.
- [x]  자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한 명 이상일 수 있다.
- [x]  우승자가 여러 명일 경우 쉼표(,)를 이용하여 구분한다.
- [x]  사용자가 잘못된 값을 입력할 경우 `IllegalArgumentException`을 발생시킨 후 애플리케이션은 종료되어야 한다.

-------------------------
## 기능 목록
### Car
- **전진 기능** - 자동차는 전진 시 총 주행 거리가 1씩 증가한다.

### CarRacing
- **전진 결정** - 참여 자동차들의 전진 여부를 랜덤으로 결정한다. 
- **최종 우승자 결정** - 참여 자동차들 중에서 총 전진 거리가 가장 큰 자동차를 우승자로 결정한다.

### CarRacingController
- **자동차 경주 게임 진행** - 사용자에게 필요한 입력을 받아 전체 시도 횟수만큼 경주를 진행한 다음, 최종 우승자를 결과를 출력한다.
- **자동차 이름 검증** - 사용자에게 입력받은 자동차 이름 문자열을 검증한다.
- **시도 횟수 검증** - 사용자에게 입력받은 시도 횟수 문자열을 검증한다.

### CarRacingUserInterface
- **사용자에게 참여 자동차들의 이름 입력 받기** - 사용자로부터 참여하는 자동차들의 이름을 입력 받는다.
- **사용자에게 시도 횟수 입력 받기** - 사용자로부터 전체 시도 횟수를 입력받는다.
- **차수별(라운드별) 진행 결과 출력** - 라운드별 게임 진행 결과를 출력한다.
- **최종 우승자 출력** - 결정된 최종 우승자를 출력한다.
- **오류 메시지 출력** - 예외 발생 시 사용자에게 오류 메시지를 출력한다.