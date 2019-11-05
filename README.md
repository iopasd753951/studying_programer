# studying_programer
개발 잔재주 공부하기 ʕ •ɷ•ʔฅ 

##### 프로그래밍공부한 것을 이해하고 내 용어로 써보기
---

# 개발 방법론

## 폭포수 모델  
- 폭포수처럼 한 번 지나가면 거슬러 갈 수 없음.
- 각 개발단계마다 확실히 매듭을 짓고, 다음 단계로 넘어감
- 관리가 쉬움

### 그러나 
- 전 단계가 수행되어 완료되기 전까지 넘어가지 못하게 제한한다.
    - ex) 완벽한 요구사항 명세 --> 기술 설계
- 개발단계마다 발생하는 피드백에 즉각적으로 반응하기 힘듦, 순차적인 흐름을 따라가기 힘듦
- 소비자들의 의해 불가능해지는 설계
    - 바뀌는 요구사항

---
## 애자일 개발 방법론

- 애자일(Agile) - 민첩한, 날렵한이라는 뜻을 가지고 있음.
- less document-oriented --> code-oriented
- 일정한 주기를 가지고 끊임없이 프로토 타입을 만들어내며 필요할 때마다 요구를 더하고 수정하여 하나의 커다란 소프트웨어를 개발

## 스크럼 개발 방법론

- 애자일 개발 방법론 중에 하나 
- **팀** 
- 개발요구 사항 목록을 작성하며 개발 목표 사항을 적는다(**Sprint Backlog**)
- 회의를 통한 반복적인 개발 주기(**Sprint**)
- 위의 내용은 개발 중에 절때 바뀌지 않음. 개발 중에 정한 원칙은 반드시 지켜야함

----

# 테스팅방법론

## 소프트웨어 테스트란

- 프로그램이나 시스템이 자신이 해야되는 일을 수행하는 믿을 과정
- 컴퓨터 소프트웨어를 실행하여 그 결과가 올바른지 판단하는 과정
---
## 단위테스트 
- 구현 단계에서 각 모듈을 구현 후 개발된 각각의 모듈을 테스트하는 것
- 단독적으로 실행할 수 있는 환경을 필요로함
---
## 통합테스트
- 단위 테스트가 완료된 후 모듈 간의 상호작용(interface)이 올바르게 되는지를 테스트
---
## 시스템 테스팅(System Testing)

- 포괄적인 테스트로 각 시스템간의 상호 연동을 중점적으로 테스트를 할 경우
- 소프트웨어는 하나의 큰 기반이 되는 컴퓨터의 구성요소라고 함

- ***전체 시스템에 대한 초기의 목적을 만족시키는가를 테스트***
- ***통합 테스트가 완료된 후에 완전한 시스템에 대해 시스템 명세에 따라 개발 되었는지를 검증하기 위한 과정***
    - 기능적인 측면에서도 검증하지만  <u>비기능적요구사항</u>도 만족 
        - 사용성, 견고성, 신뢰성, 성능, 안정성, 보안성

#### 시스템 테스팅이 추구하는 것

- 구성요소들이 서로서로, 시스템적으로 상호작용하는 것을 확인하기 위해 주변장치를 포함하여 전체적으로 통합된 어플리케이션들을 테스팅함
    - End to End senario

- 모든 입력테스팅을 검증함
- 사용자의 경험을 테스팅함

---
### 인수테스트

- 사용자의 요구사항을 만족하는 가를 확인하는 테스트

- 사용자의 입장에서 실제 사용자의 환경에서 테스트한다.

- 시스템테스트에서 사용한 테스트 케이스들을 이용할 수 있다.
    1. 알파 테스트 : 사용자의 의해 테스트되지만 개발자의 환경에서 통제된 채 테스트
    2. 베타 테스트 : 소프트웨어를 일정 수의 사용자들에게 사용하고 피드백을 받는 테스트 (개발자는 참여하지않는다.)
---
## 소프트웨어 테스팅 계층 구조

![test_structer](https://user-images.githubusercontent.com/41977701/68202139-7ae73d00-0006-11ea-93d1-dda6ce929593.png)

- 인수 테스팅
- 시스템 테스팅 
- 통합 테스팅 
- 단위 테스팅
---
## Performance Test
- 시스템의 요소가 특정 상황에서 어느정도의 성능을 보이는지를 측정하는 테스트

#### 목적
    어플리케이션의 결함을 찾는 목적이 아님.
    성능에 대한 정확하고 면밀한 모니터링을 진행

## Load Test

- 임계치의 한계에 도달할 떄까지 시스템에 부하를 꾸준히 증가시키는 것

## Stress Test 
- 시스템이 과부하 상태에서 어떻게 작동하는지를 검사하는 테스트


#### 목적
    시스템의 실패 확인 및 모니터링 과정 테스트
    정보 또는 보안상의 문제 노출 테스트
    장애 조치와 복구 절차의 테스트


## 블랙박스 테스트
- 사용자가 소프트웨어 또는 제품에 대한 요구사항과 결과물이 일치하는 지 확인하기 위한 테스트 기법
- *화이트박스 테스팅* 과는 반대의 개념으로 외부적으로 테스트하는 개념이 크다.

###### 19/ 11/ 05
