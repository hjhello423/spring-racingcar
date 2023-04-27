# jwp-racingcar

# 1단계 - 스프링 프레임워크 적용

## 미션 소개

이 미션은 자동차 경주 게임을 웹 애플리케이션으로 전환하고 DB를 연동하는 미션입니다.  
구현된 자동차 경주 게임 코드를 가져와서 웹으로 전환하고 DB와 연동하여 기록을 저장하고 조회할 수 있도록 개발해야 합니다.

## 요구사항

* 웹 요청/응답 구현하기
    -[x] '/plays' endpoint 구현
        -[x] request 구현
        -[x] response 구현
* 비즈니스 구현
    * 플레이어
        - [x] 플레이어 이름은 쉼표(,)를 기준으로 구분
        - [x] 자동차는 자신의 위치를 가지고 있음
    * 자동차 게임
        - [x] 게임 플레이 횟수를 입력받아 플레이 횟수만큼 게임을 반복 진행
        - [ ] 전진하는 조건은 0에서 9 사이에서 random 값을 구한 후 random 값이 4 이상일 경우 전진하고, 3 이하의 값이면 멈춤
        - [x] 자동차 경주 게임을 완료한 후 우승자를 구함
        - [x] 우승자는 한 명 이상일 수 있음
        - [x] 우승자가 여러명일 경우 ,를 이용하여 구분

* H2 DB를 연동
    -[x] 자동차 경주 게임의 플레이 이력을 DB에 저장
        -[x] 플레이 횟수(trialCount)
        -[x] 플레이어 별 최종 이동 거리 (이름(name), 최종 위치(position))
        -[x] 우승자(winners)
        -[x] 플레이한 날짜/시간
