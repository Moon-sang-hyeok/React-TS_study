# 01_React_structure


| 구성 요소 | 설명 |
| --- | --- |
| 컴포넌트 | UI를 구성하는 독립적이고 재사용 가능한 코드 조각 |
| Props | 부모 컴포넌트에서 자식 컴포넌트로 데이터를 전달하는 읽기 전용 속성 |
| State | 컴포넌트 내부에서 관리되는 변경 가능한 데이터 |
| JSX | JavaScript를 확장한 문법으로, UI를 설명하는 데 사용 |
| 생명주기 메서드 | 컴포넌트의 마운팅, 업데이트, 언마운팅 단계에서 실행되는 메서드 |
| Hooks | 함수형 컴포넌트에서 상태와 생명주기 기능을 사용할 수 있게 해주는 함수 |
| Context API | 컴포넌트 트리 전체에 데이터를 제공하는 방법 |
| 라우팅 | 다중 페이지 애플리케이션에서 페이지 간 네비게이션을 관리 |

<br>

## 컴포넌트 기반 아키텍처

- React의 핵심은 컴포넌트 기반 아키텍처
- 사용자 인터페이스를 독립적이고 재사용 가능한 조각으로 나누어 구성

- **함수형 컴포넌트**: 간단하고 상태가 없는 컴포넌트를 함수로 정의
- **클래스형 컴포넌트**: React.Component를 상속받아 더 복잡한 기능과 생명주기 메서드를 관리

<br>

## 단방향 데이터 흐름

데이터는 부모 컴포넌트에서 자식 컴포넌트로 단방향으로 흐름

<br>

## 가상 DOM (Virtual DOM)

성능 최적화를 위해 실제 DOM의 가벼운 복사본을 사용

<br>

## JSX

JavaScript를 확장한 문법으로, UI 컴포넌트를 설명하는 데 사용

<br>

## 상태 관리

컴포넌트 내부에서 관리되는 변경 가능한 데이터인 상태(state)와 부모 컴포넌트에서 전달받는 읽기 전용 속성인 props를 사용

<br>

## 디렉토리 구조

해당 구조를 통해 React는 효율적이고 유지보수가 용이한 웹 애플리케이션을 구축함

| 디렉토리/파일 | 설명 |
|---------------|------|
| src | 주요 소스 코드 |
| src/components | 재사용 가능한 UI 컴포넌트 |
| src/pages | 주요 페이지 또는 라우트 |
| src/assets | 이미지, 스타일시트 등의 정적 파일 |
| public | 공개적으로 접근 가능한 정적 자산 |
| App.js | 애플리케이션의 루트 컴포넌트 |
| index.js | 애플리케이션의 진입점 |

<br>

## Vue와의 차이점

| 특성 | Vue | React |
| --- | --- | --- |
| 구문 | 콧수염 구문 {{ }} | 중괄호 { } |
| 기반 | HTML **템플릿** | **JSX (JavaScript XML)** |
| JavaScript 표현식 | 제한된 표현식 지원 | 모든 **JavaScript 표현식 지원** |
| 컨텍스트 | Vue 인스턴스의 데이터 컨텍스트 | 컴포넌트의 JavaScript 컨텍스트 |
| 최적화 | Vue 프레임워크에 의해 처리 | JavaScript 엔진에 의해 직접 최적화 가능 |
| HTML과의 유사성 | 높음 | 낮음 |
| 유연성 | 상대적으로 낮음 | 높음 |
| 학습 곡선 | 상대적으로 낮음 | 상대적으로 높음 |
| 디자인 철학 | **HTML 템플릿 중심** | JavaScript 중심 |