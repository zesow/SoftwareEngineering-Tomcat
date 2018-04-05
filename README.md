# SoftwareEngineering-Tomcat
2018-1 소프트웨어 공학 주제로 정한 톰캣 요구사항 분석입니다.


## Business Goal
- 웹서버에서 자바를 이해할 수 있는 엔진이 필요
  - 톰캣은 웹 서버와 연동하여 실행할 수 있는 자바 환경을 제공하여 자바 서버 페이지(JSP)와 자바 서블릿이 실행할 수 있는 환경을 제공한다.

## Constraint
- Business Constraints
  - 다른 유료DB와 달리 기술 지원을 받을 수 없다.
  
- Technical Constraints
  - Java만 인식 가능하므로 php 등 다른 언어는 apache에서 해당 엔진을 호출하여 상호 보완적 동작을 수행하도록 한다.
  - 정적 파일(html,css,js…) 의 처리는 Apache Web Server 이 더 빠르므로 결합해서 사용한다.

## Functional Requirements
1. Manager 웹 응용 프로그램은 요청 URI를 통해 전체적으로 표현되는 명령으로 Tomcat을 관리하기위한 간단한 HTTP 기반 인터페이스를 제공 (HTTP 트랜잭션을 생성 할 수 있는 도구로 관리 명령을 스크립팅 하려는 환경에서 유용)

2. 사람이 관리 기능과 상호 작용할 수 있는 GUI와 유사한 사용자 인터페이스를 제공

3. Tomcat을 관리하기위한 운영 명령은 SOAP 메시지 형식을 사용하는 웹 서비스로 제공

4. Tomcat을 관리하기위한 작업 명령은 JMX API를 통해 사용 가능하게 만들어, 관리 콘솔에 통합

5. JINI, RMI 및 CORBA와 같은 다른 원격 액세스 API를 사용하여 관리 기능에 접근 할 수 있도록 함

## Quality Attribute Scenario

|  <center>분류</center> |  <center>내용</center>
|:--------:|:--------|
|**Requirement-ID** | QA_01|
|**Category** | avalibility|
|**Concern** | 최신 코드 반영|
|**Source** | 시스템|
|**Stimulus** | 소스 코드 변경|
|**Environment** | 소스 코드 변경|
|**Artifacts** | 시스템 |
|**Response** | 톰캣 재부팅.|
|**Response Measure** | 10초마다 변경 사항 감지.|
|**Priority** | 3 |
|**Description** | 주기적으로 코드를 감시하는 도중 코드 변경 시 자동으로 재시작하여 시스템을 최신으로 유지한다. |

|  <center>분류</center> |  <center>내용</center>
|:--------:|:--------:|
|**Requirement-ID** | QA_02|
|**Category** | 이것이 내용입니다.|
|**Concern** | 이것이 내용입니다.|
|**Source** | 이것이 내용입니다.|
|**Stimulus** | 이것이 내용입니다.|
|**Environment** | 이것이 내용입니다.|
|**Artifacts** | 이것이 내용입니다.|
|**Response** | 이것이 내용입니다.|
|**Response Measure** | 이것이 내용입니다.|
|**Priority** | 이것이 내용입니다.|
|**Description** | 동시접속자.|

|  <center>분류</center> |  <center>내용</center>
|:--------:|:--------:|
|**Requirement-ID** | QA_02|
|**Category** | 이것이 내용입니다.|
|**Concern** | 이것이 내용입니다.|
|**Source** | 이것이 내용입니다.|
|**Stimulus** | 이것이 내용입니다.|
|**Environment** | 이것이 내용입니다.|
|**Artifacts** | 이것이 내용입니다.|
|**Response** | 이것이 내용입니다.|
|**Response Measure** | 이것이 내용입니다.|
|**Priority** | 이것이 내용입니다.|
|**Description** | 주기적인 백업 발생.|

## Quality Attribute Utility Tree
|  <center>속성</center> |  <center>우려</center> |   <center>시나리오</center> |  <center>(I,R)</center> |  <center>우선순위</center> |
|:--------:|:--------:|:--------:|:--------:|:--------:|
|**Description** | 이것이 내용입니다.| 이것이 내용입니다.| 이것이 내용입니다.| 이것이 내용입니다.|
|**Description** | 이것이 내용입니다.| 이것이 내용입니다.| 이것이 내용입니다.| 이것이 내용입니다.|
