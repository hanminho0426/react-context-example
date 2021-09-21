#Context API

- 하위 컴포넌트 전체에 데이터를 공유하는 법
  - 데이터를 Set 하는 놈
    - 가장 상위 컴포넌트 => 프로바이더
  - 데이터를 Get 하는 놈
    - 모든 하위 컴포넌트에서 접근가능
      - 컴슈머로 하는 방법
      - 클래스 컴포넌트의 this.context로 하는 방법
      - 펑셔널 컴포넌트의 useContext로 하는 방법

## 데이터를 Set 하기

1. 일단 컨텍스트를 생성한다.
2. 컨텍스트.프로바이더를 사용한다.
3. value를 사용

## 데이터를 Get 하기 (1) = Consumer

1. 컨텍스트를 가져온다.
2. 컨텍스트, 컨슈머를 사용한다.
3. value를 사용

## 데이터를 Get 하기 (2) = class

1. static contextType에 컨텍스트를 설정한다.
2. this.context => value 이다.

## 데이터를 Get 하기 (3) = functional

1. useContext로 컨텍스트를 인자로 호출한다.
2. useContext의 리턴이 value이다.
