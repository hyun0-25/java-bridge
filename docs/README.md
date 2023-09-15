# 구현할 기능 목록

- [ ]  출력: `다리 건너기 게임을 시작합니다.`
    - [ ]  출력: `다리의 길이를 입력해주세요.`
        - [ ]  다리 길이 입력 (3이상 20이하의 숫자)
            - [ ]  올바른 값이 아니면 예외 처리

              ex) 3

    - [ ]  출력: `이동할 칸을 선택해주세요. (위: U, 아래: D)`
        - [ ]  라운드마다 플레이어가 이동할 칸을 입력 (U 또는 D)
            - [ ]  올바른 값이 아니면 예외 처리
        - [ ]  출력: `다리 모양`

          ex)

           ```
           [ O | X ]
           [   |   ]
           ```

    - [ ]  게임실패
        - [ ]  출력: `게임을 다시 시도할지 여부를 입력해주세요. (재시도: R, 종료: Q)`
            - [ ]  게임 재시도/종료 여부 입력 (R-재시도 또는 Q-종료)
                - [ ]  올바른 값이 아니면 예외 처리
            - [ ]  R-재시도
                - [ ] 
            - [ ]  Q-종료
                - [ ]  출력: `최종 게임 결과`
                - [ ]  출력: 다리 모양

               ```
               [ O |   |   ]
               [   | O | O ]
               ```

                - [ ]  출력: `게임성공 여부: 성공 or 실패`
                - [ ]  출력: `총 시도한 횟수: 값`

# 클래스 및 함수

- Application
    - main()
        - 프로그램 실행
- BridgeGame
    - move()
    - retry()
- BridgeMaker
    - BridgeMaker( `BridgeNumberGenerator bridgeNumberGenerator`)
    - makeBridge( `int size`)
- BridgeRandomNumberGenerator (implements BridgeNumberGenerator)
    - generate()

### Interface

- BridgeNumberGenerator
    - generate()

### View

- InputView
    - readBridgeSize()
    - readMoving()
    - readGameCommand()
- OutputView
    - printMap()
    - printResult()

# 예외처리