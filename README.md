# mims-frontend
Medical Information Monitoring Service - Frontend

## 세나클 소프트 인턴 프로젝트

### 프로젝트 소개

#### 서비스명 : MIMS(Medical Information Monitoring Service)
![MIMS_logo](https://user-images.githubusercontent.com/37138188/187113565-99506f26-9a52-421b-b65a-644c0e5f5085.png)

#### 기간 : 22.07.25. ~ 22.08.31.

#### 인원 : 2명(Full-Stack)

#### 역할
- 백엔드 개발
- 프론트 개발
- PPT 및 가이드라인 제작

#### 느낀점
- 테스트 코드 중요성 -> 데이터 PoC
- 의사소통의 중요성 -> 이해하는 부분이 달라서 구현에 문제가 생기는 경우
- 코드 모듈화의 중요성 -> 테스트 코드 짤 때, 모듈화를 신경쓰지 않고 짰더니 결합도가 높아져서, 분리가 힘든 상황을 맞딱드림. 테스트 코드를 짜더라도, 모듈화를 잘하자.
- DB 엔티티 설계 -> 인덱싱을 안 걸꺼면 여러 칼럼들 Json으로 관리할 것인지? 등등
- 테스크 스케줄링 하기 -> 주기적으로 실행하고 하는 process로 테스크를 만들고 스케줄링으로 관리
rout
### 프로젝트 개요

EMR 서비스
- 가이드 지침 + 공단 지침 -> 데이터
- 청구나 심사가 오픈되어 있고 추가되거나 수정되는 부분을 계속 반영해야 함
- EX) 코로나 검사에 대한 공제가 새로 생김. 이것이 고지 형태로 나옴.
- 이런 변화된 부분들을 빠르게 서비스에 반영하는 것이 중요.
- 이런 고지들은 여러 기관 사이트에 분포되어 있음.

**각 사이트별 추가/변경되는 고지들을 모니터링 하는 서비스의 필요성**

### 기술
Backend
- Spring Boot(v.2.7.2)
- MySQL
- Spring JPA
- MapStruct
- QueryDSL
- Selenium

Frontend
- React.js
- Recoil
- Scss
- Axios
- React-icons
- Http-proxy-middleware

### 이슈 및 트러블 슈팅

1. 파일 및 폴더구조
```
- src
    - compontents
        - common
        - MonitoringItemInfo
        - SearchContentMonitoringItem
        - SearchJsonApiMonitoringItem
        - SearchTagMonitoringItem
        - UserInfo
    - recoil
    - routes
    - styles
    - utils
```

**리액트 쿼리 qs window.location.search**
- https://bloodstrawberry.tistory.com/569

**리액트 여러가지 검색 할 때**
- https://velog.io/@jhs000123/%EB%A6%AC%EC%95%A1%ED%8A%B8-%EC%97%AC%EB%9F%AC%EA%B0%9C%EC%9D%98-input-%EC%A0%9C%EC%96%B4%ED%95%98%EA%B8%B0
- https://goddino.tistory.com/296

**리액트 baseUrl 설정**
- https://mia-dahae.tistory.com/137

**useEffect 무한루프**
- https://velog.io/@tjehdgur1500/useEffect-%EB%AC%B4%ED%95%9C%EB%A3%A8%ED%94%84

**Checkbox 구현**
- https://goddino.tistory.com/229

**JS ES6 Map Set**
- https://velog.io/@silverj-kim/Javascript-ES6-Map-Set

**JS Filter 및 Find**
- FILTER : https://7942yongdae.tistory.com/49
- FIND : https://bbaktaeho-95.tistory.com/40

**리액트 경로이동 navigate 훅**
- https://curryyou.tistory.com/476

**리액트 갓디노 - 체크박스 토글 기능 구현**
- https://goddino.tistory.com/229

**리액트 갓디노 - 게시판 만들기 #1 #2**
- https://goddino.tistory.com/154?category=902116
- https://goddino.tistory.com/155
