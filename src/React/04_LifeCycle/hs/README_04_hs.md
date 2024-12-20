# 04_라이프사이클

## 강의 목차

- '한입 리액트' : 라이프사이클
- '리액트 완벽 가이드' : 리액트 핵심 - 컴포넌트, JSX, 속성, 상태 등 / 리액트 핵심 - 심화 단계

---

### 라이프사이클이란?

- 생애 주기
    - Mount
        - 컴포넌트가 탄생하는 순간
        - 화면에 처음 렌더링 되는 순간
        - 서버에서 데이터를 불러오는 작업
    - Update
        - 컴포넌트가 다시 렌더링 되는 순간
        - 리렌더링 될 때
        - 어떤 값이 변경되었는지 콘솔에 출력
    - UnMount
        - 컴포넌트가 화면에서 사라지는 순간
        - 렌더링에서 제외 되는 순간
        - 컴포넌트가 사용하던 메모리 정리

### UseEffect

- 리액트 컴포넌트의 사이드 이펙트를 제어하는 새로운 리액트 훅
- 부수적인 효과, 파생되는 효과를 제어
- 어떤 값이 변경되었을 때 원하는 동작을 수행하도록 만들 수 있다
- 첫 번째 인수로는 콜백함수, 두 번째 인수로는 배열
    - 배열에 들어가 있는 값이 바뀌게 되면, 첫 번째 인수로 전달한 콜백함수를 실행
    - 해당 배열엔 변경을 확인 할 값을 넣어준다, 여러 개 넣어도 됨
    - `useEffect(() => {}, [count])`
    - 배열 → 의존성 배열 / dependency array → deps

### UseEffect로 라이프사이클 제어하기

- 마운트
    - `useEffect(() => {}, [])`
- 업데이트
    - `useEffect(() => {})`
- 언마운트
    - `useEffect(() => { return () => {} }, [])`  → 클린업, 정리함수