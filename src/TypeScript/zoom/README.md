# TypeScript - 코딩 앙마 STUDY

날짜: 2025년 1월 3일

# 1.  **타입스크립트를 쓰는 이유**

## 1. 🤔 타입스크립트를 사용하는 이유

- 타입스크립트는 자바스크립트로 변환되어야 하며, 이를 통해 여러 가지 장점을 제공한다.
- 예를 들어, 잘못된 인자 타입을 사용하면 자바스크립트는 오류를 사전 단계에서 알리지 않기 때문에 개발자가 실수할 수 있다.
- 이러한 문제는 타입스크립트를 통해 해결할 수 있으며, 이는 개발자가 예상하지 못한 오류를 런타임 이전에 발견하도록 돕는다.

## 2. 💻 타입스크립트의 정적 타입 언어 특성

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/5oGAkQsGWkc/18.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/5oGAkQsGWkc/18.jpg)

- **타입스크립트는 정적 타입 언어**로, 컴파일 시점부터 타입 검사가 이루어진다.
- 코드 작성 시 초기 고려 사항이 많아지지만 이는 코드 작성의 안정성을 높이고, **작업 속도를 빠르게** 하는 데 기여한다.
- 타입스크립트의 특징으로 인해 **신뢰할 수 있는 코드를 작성**할 수 있다.

## 3. ✍️ 타입스크립트 플레이그라운드 활용하기

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/5oGAkQsGWkc/18.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/5oGAkQsGWkc/18.jpg)

| 항목 | 설명 |
| --- | --- |
| **타입 추론** | - 타입을 알 수 없을 때 기본적으로 'any' 타입으로 판단
- 'any' 타입 사용은 가능한 자제해야 함 |
| **타입 지정** | - 특정 타입 지정으로 불필요한 오류 메시지 감소
- 예: number 타입으로 고정 |
| **에러 감지** | - 인수의 개수가 맞지 않을 때 에러 메시지 출력
- 개발자의 실수를 감지하고 알림 |
| **코드 품질** | - 불필요한 타입 사용 자제
- 하나의 타입으로 고정하여 코드 품질 향상 |
| **함수 정의 예시** | - add 함수: 숫자 타입의 인수 요구
- 타입 정의 후 원하는 타입 명시 필요 |
| **타입 변경 효과** | - 'any' 타입 제거 후 number로 고정 시, 문자열 입력 시 에러 발생 |
| **매개변수 처리** | - 필요한 인수 개수와 다를 경우 에러 메시지 출력
- 타입이 맞지 않을 경우에도 에러 발생 |

## 4. 🛠️ 타입 지정의 중요성

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/5oGAkQsGWkc/326.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/5oGAkQsGWkc/326.jpg)

- 함수를 만들 때 **인수들의 타입을 지정**하는 방법이 있으며, 이는 코드의 안정성을 높인다.
- 매개변수의 타입을 명확히 지정함으로써 다른 사람이 만든 함수를 사용할 때 어떤 타입으로 전달해야 하는지를 쉽게 이해할 수 있다.
- 코드의 **오류를 미리 감지**할 수 있어 수정해야 할 부분을 사전에 알아차릴 수 있다.
- 타입 스크립트는 브라우저에서 코드를 실행할 때 오류가 있는 코드를 그대로 보여 주며, 이해를 돕는다.
- 사용법을 명확하게 알림으로써 **제대로된 사용**이 가능하게 한다.

# 2. **기본 타입 - 타입스크립트 강좌**


## 1. 💡 타입스크립트의 기본 타입

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/70w82P-KiVM/0.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/70w82P-KiVM/0.jpg)

- 문자 타입은 스트링으로 선언하며, 변수에 값을 쌓을 수 있다.
- 스트링이 아닌 다른 타입으로 선언할 경우 에러가 발생한다.
- 타입스크립트는 타입을 자동으로 인식하여 명시적으로 선언할 필요가 없다.
- 다양한 타입에 대해 추가적으로 살펴볼 예정이다.

## 2. 📊 타입스크립트의 기본 타입 이해하기

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/70w82P-KiVM/46.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/70w82P-KiVM/46.jpg)

- 불린 타입은 **true** 또는 **false** 값으로, 기본적인 논리 연산을 수행하는데 사용된다.
- 배열의 각 요소는 숫자로 이루어져 있으며, 각각의 값을 개별적으로 접근하고 처리할 수 있다.
- **문자열**에 대해서는 `trim()` 메서드를 사용하여 공백을 제거할 수 있다.
- 인덱스 별로 타입이 다를 수 있으며, 예를 들어 **문자열**과 **넘버**를 같이 사용할 수 있다.
- 타입스크립트는 타입을 사전에 정의함으로써 코드 작성 시 에러를 피할 수 있게 도와준다.

## 3. 💻 타입스크립트에서의 기본 타입 설명

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/70w82P-KiVM/163.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/70w82P-KiVM/163.jpg)

- **void**는 함수에서 아무것도 반환하지 않을 때 주로 사용되며, 이는 입력 시 아무것도 바라지 않는 상황을 나타낸다.
- void는 항상 **에러를 반환**하거나 영원히 끝나지 않는 암시적인 타입으로 사용될 수 있다.
- 이넘 타입은 비슷한 값끼리 **묶여** 있다는 특징이 있다.

## 4. 🖥️ 이넘(Enums) 사용법과 활용

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/70w82P-KiVM/204.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/70w82P-KiVM/204.jpg)

- **이넘은** 값이 자동으로 `0부터 1씩 증가하며 할당`된다. 기본적으로 첫 번째 값은 0으로 시작된다.
- **수동으로 값을 지정**할 수 있으며, 예를 들어 iOS를 10으로 바꾸면 다른 값들이 자동으로 조정된다.
- **이넘은 숫자뿐만 아니라 문자열** 값도 입력할 수 있고, 이를 통해 다양한 값을 지정할 수 있다.
- **특정 값들만 입력**하도록 제한해주고 싶을 때 이넘을 사용하면 유용하다.
- **이넘을 통해 코드의 가독성과 관리**가 용이해지며, 특정 값들에 대한 공통점을 강조할 수 있다.

## 5. 📊 타입스크립트의 null과 undefined

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/70w82P-KiVM/321.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/70w82P-KiVM/321.jpg)

- **null**은 특별한 값으로, 변수에 **값이 없음**을 나타낸다.
- **undefined**는 변수가 선언되었으나 값이 할당되지 않은 상태를 의미한다.
- null과 undefined 각각의 용도를 이해하고 사용할 수 있다.

# 3. 인터페이스


## 1. 🖥️ 인터페이스와 옵셔널 프로퍼티

- 인터페이스는 객체에 특정 속성 값을 정의하여 에러를 방지할 수 있도록 도와준다.
- 유저 타입을 선언하면서 name과 age 프로퍼티를 정의하고 임의의 값을 넣을 수 있지만, 추가적인 속성인 gender는 정의되지 않았으므로 오류가 발생한다.
- 옵션 속성을 만들기 위해서에는 물음표를 붙여 주어 선택적 속성으로 설정할 수 있으며, 이를 통해 에러를 해결할 수 있다.

## 2. 🔍 읽기 전용 프로퍼티와 인터페이스의 활용

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/OIMPLNICzoc/34.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/OIMPLNICzoc/34.jpg)

- **readonly** 키워드를 사용하면 값에 접근은 가능하지만 수정은 불가능하다.
- 인터페이스에서 **벌수번호**는 **number** 타입으로 정의되며, 'in'을 사용하면 자동완성 기능이 제공된다.
- **수량** 프로퍼티는 초기 입력 후 수정이 가능하지만, 특정 조건에서 에러가 발생하지 않는다.
- `최초 생성 시 할당만 가능하며, 이후에는 수정할 수 없는 점이 읽기 전용 속성의 특징이`다.

## 3. 📊 타입스크립트에서의 속성 관리 방법

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/OIMPLNICzoc/53.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/OIMPLNICzoc/53.jpg)

| 특징 | 설명 | 효과 |
| --- | --- | --- |
| 옵셔널 프로퍼티 | 여러 점수를 기록하기 위해 사용되며, 특정 속성이 필수가 아님 | 에러 없이 정보 전달 가능 |
| 문자열 인덱스 시그니처 | 다양한 키와 값의 조합을 통해 여러 프로퍼티를 정의할 수 있음 | 성적을 효과적으로 관리 가능 |
| 스코어 타입 정의 | A, B, C, F로 지정된 타입 | 타입 안정성 제공 |
| 스코어 타입 활용 | 스트링 타입 대신 스코어 타입을 사용하여 데이터의 정확성을 높임 | 잘못된 데이터 입력 방지 |
| 입력 값 형식 제한 | 특정 스트링 형식에 맞춰 입력해야 함 | 데이터 무결성 보장 |
| 잘못된 데이터 구조 | 다른 데이터를 입력하거나 잘못된 구조의 데이터를 사용하면 에러 발생 | 에러를 통해 잘못된 입력을 방지 |

## 4. ✍️ 인터페이스를 활용한 함수 정의

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/OIMPLNICzoc/311.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/OIMPLNICzoc/311.jpg)

- **인터페이스**를 통해 함수의 파라미터와 리턴값을 정의할 수 있다.
- `함수의 정의가 인터페이스와 일치하지 않을 경우 **타입 에러**`가 발생한다.
- 화살표 함수로도 간단하게 정의할 수 있으며, 조건부 로직을 통해 **true** 또는 **false**를 반환하는 것이 가능하다.

## 5. 🚗 인터페이스를 통한 클래스 정의

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/OIMPLNICzoc/448.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/OIMPLNICzoc/448.jpg)

- 인터페이스를 사용하여 클래스를 **정의**할 수 있으며, 이때는 **implements** 키워드를 사용해야 한다.
- 모든 속성 값을 입력해야 하며, 이를 통해 **에러**를 예방할 수 있다.
- 인터페이스 사용을 통해 코드의 **재사용성**이 향상된다.

## 6. ✨ 인터페이스의 확장 및 활용

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/OIMPLNICzoc/537.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/OIMPLNICzoc/537.jpg)

- **인터페이스**는 확장이 가능하여, 다른 인터페이스의 속성을 **상속**받을 수 있다.
- **예를 들어**, 특정 속성을 포함한 인터페이스를 만들고 추가 속성을 더할 수 있다.
- 여러 개의 인터페이스를 **동시에 확장**하는 것이 가능하며, 이를 통해 보다 복잡한 구조를 만들 수 있다.

# 4. 함수


## 1. ✏️ 함수 타입 정의 및 옵셔널 매개변수

- 함수의 매개 변수에는 타입을 정의할 수 있으며, 기본적으로 필수 매개 변수를 요구한다.
- TypeScript에서는 옵셔널 매개변수를 사용하여 매개 변수를 선택적으로 입력할 수 있도록 지원하며, 이를 위해 물음표(?)를 붙여 명시적으로 처리한다.
- 선택적 매개변수는 입력을 해도 되고, 하지 않아도 되는 항목으로, 이때 주의할 점은 선택적 매개변수가 필수 매개변수보다 앞에 입력될 수 없다는 것이다.

## 2. 🧮 나머지 매개 변수의 활용

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/prfgfj03_VA/31.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/prfgfj03_VA/31.jpg)

- **add 함수**는 숫자들을 더해준 값을 반환하는 기능을 가지고 있다.
- **레스트 파라미터**는 매개 변수의 개수가 다를 때 유용하게 사용된다.
- 전달받은 매개 변수는 **배열**로 처리할 수 있다.
- 타입스크립트에서는 매개 변수를 배열 형태로 **전달**할 수 있다.

## 3. 🐱 TypeScript에서 this와 함수의 활용

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/prfgfj03_VA/31.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/prfgfj03_VA/31.jpg)

- **this**와 관련된 내용은 가변적일 수 있으며, 특정 객체에 의해 정의될 수 있다.
- 매개변수를 통해 **this**를 명시적으로 정의하고, 해당 타입을 입력해야 한다.
- 매개변수를 적절히 전달하면 오류가 발생하지 않으며, 그 순서를 명확히 해야 한다.
- 예제를 통해 여러 매개변수가 올바르게 처리되는 과정을 보여준다.

## 4. ✨ 함수 오버로드와 타입 반환

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/prfgfj03_VA/368.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/prfgfj03_VA/368.jpg)

- 전달받은 매개변수의 타입에 따라 함수의 리턴 타입이 달라지며, 개체이거나 문자열이 될 수 있다.
- 함수 오버로드를 통해 매개변수의 개수나 타입에 따라 다른 동작을 기술할 수 있으며, 이를 동일한 함수 이름으로 작성해야 한다.
- 타입이나 개수에 따라 외부 변수의 동작 방식이 달라져야 할 때, 함수를 오버로드하여 해결할 수 있다.

# 5. 리터럴 / 유니온 / 교차타입


## 1. ✏️ 문자열 및 숫자 리터럴의 정의와 예시

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/QZ8TRIJWCGQ/60.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/QZ8TRIJWCGQ/60.jpg)

- **문자열 리터럴**은 정해진 문자열 값을 가지는 것으로 정의된다.
- 일부 값이 예외적으로 허용되지 않아 **에러가 발생**하는 경우가 있다.

## 2. 🚗 유니언 타입의 이해

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/QZ8TRIJWCGQ/106.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/QZ8TRIJWCGQ/106.jpg)

- 유니언 타입은 **`number`** 또는 **`string`**과 같은 여러 형식을 조합하여 사용할 수 있다.
- 두 개의 인터페이스인 **`Car`**와 **`Mobile`**이 있으며, 각각 출발과 전화를 연결하는 기능을 가지고 있다.
- 유니언 타입을 활용하여 **함수** 구현 시, 특정 인터페이스에 속하는지 검증해야 하며, 이를 통해 **에러**를 방지할 수 있다.
- 함수를 호출하기 전에 유니언 타입의 객체가 **`Car`**인지 확인하는 것이 중요하다.
- `start` 메소드는 **`Car`** 인터페이스에만 존재하므로, 적절한 타입 체크가 선행되어야 한다.

## 3. 🔑 식별 가능한 유니온 타입의 활용

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/QZ8TRIJWCGQ/106.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/QZ8TRIJWCGQ/106.jpg)

- **식별 가능한 유니온 타입**을 사용하면 동일한 속성을 다르게 주어 두 개의 인터페이스를 함께 사용할 수 있다.
- 특정 타입을 프린트할 경우, `T`는 '카'로 인식되며, 이는 모바일과 구별되는 특성이다.
- 이러한 속성의 타입을 서로 분할할 수 있는 요소가 **식별 가능한 유니온 타입**이다.

## 5. 🛠️ 교차 타입의 개념 및 활용

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/QZ8TRIJWCGQ/257.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/QZ8TRIJWCGQ/257.jpg)

- **교차 타입**은 여러 타입을 합쳐서 활용하는 방법이다.
- 영어로는 **'인터섹션 타입'**이라고 불리며, 여러 프로퍼티를 포함할 수 있다.
- 예를 들어, 'a 또는 b'와 같이 둘 중 하나를 선택하는 것은 **'또는'**을 의미하며, 프로퍼티는 **'&'**로 표현된다.

## 6. 🔍 타입 합성과 속성 정의

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/QZ8TRIJWCGQ/290.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/QZ8TRIJWCGQ/290.jpg)

- 모든 속성을 가지려면 필수 속성을 제대로 정의해야 한다.
- 각 인터페이스의 속성을 정확하게 작성해야 한다.
- 여러 타입을 하나로 **합치는 역할**을 수행하며, 필요한 모든 기능을 포함한 타입을 생성한다.

# 6. 클래스


## 1. 📝 타입스크립트 클래스 선언 및 작성 방법

- 타입스크립트에서 클래스를 작성할 때에는 반드시 멤버 변수를 선언해야 하며, 선언하지 않으면 타입 에러가 발생한다.
- 클래스에서 생성자를 정의할 때는 각 프로퍼티의 타입을 명시해야 하며, 예를 들어 "칼라"의 경우에는 스트링 타입으로 지정해야 한다.
- 멤버 변수를 미리 선언하지 않으려면 접근 제한자나 도우미 유형을 활용할 수 있으며, 예를 들어 "컬러" 앞에 `public`을 붙여서 사용할 수 있다.

## 2. 🏷️ 클래스 접근 제어자와 상속

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/17Oh028Jpis/88.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/17Oh028Jpis/88.jpg)

- **퍼블릭**으로 선언된 프로퍼티는 자식 클래스와 인스턴스에서 접근할 수 있다.
- **프라이빗**으로 선언된 프로퍼티는 클래스 내부에서만 접근 가능하며, 자식 클래스에서는 사용할 수 없다.
- **프로텍티브** 접근 제어자는 자식 클래스 내부에서는 접근할 수 있지만, 클래스 인스턴스에서는 사용할 수 없다.
- 일반적으로 접근 제어자를 명시하지 않으면 기본적으로 **퍼블릭**으로 간주된다.
- **#** 기호를 사용하여 프로퍼티를 프라이빗으로 표시할 수 있으며, 이는 문법적으로 간편한 선택일 뿐 기능상 차이는 없다.

## 3. ✨ 클래스의 동적 및 정적 멤버

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/17Oh028Jpis/305.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/17Oh028Jpis/305.jpg)

- T 프로퍼티를 사용하면 **동적 멤버 변수**를 생성할 수 있다.
- 동적 멤버 변수는 클래스의 점(.)으로 접근할 수 있다.
- 정적 멤버 변수는 **static**으로 선언해야 하며, 이 경우 클래스명을 사용해야 한다.
- 정적 멤버 변수에 접근할 때는 `this`를 사용하지 않고 클래스명을 넣어야 하며, 이를 통해 에러가 발생하지 않는다.
- 에러가 사라지면 정적 멤버 변수 접근이 성공한 것이다.

| 접근 제어자 | 클래스 내부 | 자식 클래스 | 같은 패키지 | 다른 패키지 |
| --- | --- | --- | --- | --- |
| public | O | O | O | O |
| protected | O | O | O | X |
| default | O | O | O | X |
| private | O | X | X | X |
- **public**: 모든 곳에서 접근 가능
- **protected**: 같은 패키지 내에서, 그리고 다른 패키지의 자식 클래스에서 접근 가능
- **default**: 같은 패키지 내에서만 접근 가능 (접근 제어자를 명시하지 않았을 때)
- **private**: 해당 클래스 내에서만 접근 가능

### 주의사항

1. 클래스에는 public과 default만 사용 가능
2. 생성자에 super()를 호출하지 않으면 컴파일 에러 발생
3. private 멤버는 자식 클래스에서 직접 접근 불가
4. 문법은 private 멤버를 정의하는 새로운 방식
5. 읽기 전용 프로퍼티 수정은 constructor 내에서만 가능

## 4. 🏗️ 추상 클래스의 개념

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/17Oh028Jpis/359.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/17Oh028Jpis/359.jpg)

- **추상 클래스**는 `abstract` 키워드를 사용하여 정의된다.
- 일반적으로 **new**를 이용해 인스턴스를 생성할 수 없고, **상속**을 통해서만 사용할 수 있다.
- 추상 클래스 내부에 있는 추상 메서드는 반드시 **상속받은 클래스**에서 구체적인 구현이 필요하다.
- 추상 클래스 메서드는 단순히 이름만 남겨줄 뿐이다.
- 추상 클래스와 그 개념이 낯설 수 있는 사람도 있을 것으로 추정된다.

## 5. 📝 추상화와 클래스의 이해

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/17Oh028Jpis/413.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/17Oh028Jpis/413.jpg)

- **추상화**는 프로퍼티나 이름만 선언하고, 구체적인 기능은 **상속받은 클래스**에서 구현하는 것을 의미한다.
- 추상 클래스를 상속받은 여러 객체들이 동일한 특성을 가질 수 있지만, 각 객체의 구체적인 기능은 다를 수 있다.

# 7. 제네릭


## 1. 🛠️ 제네릭의 활용

- 제네릭은 클래스, 함수, 인터페이스를 다양한 타입으로 사용하는 방법이다.
- 타입 파라미터를 선언한 후, 생성 시점에 사용할 타입을 결정하는 방식으로 동작한다.

## 2. 📏 제네릭의 필요성과 사용법

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/pReXmUBjU3E/14.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/pReXmUBjU3E/14.jpg)

- 'getSize' 함수는 배열의 **크기**를 반환하는 기능을 수행한다.
- 배열의 타입에 따라 에러가 발생할 수 있으며, 이를 유니언 타입이나 오버로드로 해결할 수 있다.
- 여러 타입을 수용하기 위해 **제네릭**을 도입하고, 이를 통해 매번 타입을 명시할 필요가 없어진다.
- 제네릭은 꺽쇠를 사용하여 정의하며, 일반적으로 'T'를 타입 파라미터로 사용한다.
- 타입 파라미터는 호출 시에 전달된 타입에 기반해 결정되며, 이를 통해 코드의 **유연성**이 증가한다.

## 3. 🛠️ 제네릭의 활용 예시.

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/pReXmUBjU3E/128.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/pReXmUBjU3E/128.jpg)

- 'options'에는 **알려지지 않은 데이터**가 들어올 수 있으며, 이는 문자열, 객체, 불린 또는 **undefined**가 될 수 있다.
- 제네릭을 사용하여 이러한 다양한 데이터 타입을 처리할 수 있으며, 이는 **타입 안전성**을 높이는 데 기여한다.
- 두 번째 **'T'**를 적어주고, 'options'는 뒤의 타입으로 연결하는 방식으로 제네릭을 구현한다.

## 4. 🔍 제네릭을 통한 객체 타입 관리

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/pReXmUBjU3E/128.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/pReXmUBjU3E/128.jpg)

- 개체 2개를 생성하며, 다양한 타입을 적용해야 하는 상황에서 에러가 발생한다.
- 첫 번째 객체는 **오브젝트**로 구성되어 있으며, 두 번째 객체는 옵션의 타입이 '스트링'이다.
- 제4의 활용으로 단일 객체를 선언하고, 다른 타입의 객체를 자유롭게 제시할 수 있다.
- 매개변수 타입 설정에서 에러가 발생할 수 있으며, 이는 모든 매개 변수의 네임이 일치하지 않을 때 나타난다.
- 타입을 적절히 설정하고, 네임이 '스트링' 객체를 확장한 형태로 명시되면 에러를 피할 수 있다.

# 8. 유틸리티

## 1. 📝 유틸리티 타입의 이해와 활용

- 'keyof' 키워드를 사용하면 유저 인터페이스의 키 값을 의미하는 형태로 받을 수 있으며, 특정한 값으로 입력하면 에러가 사라진다.
- 프로퍼티를 모두 옵션으로 바꾸는 방법은 유틸리티 타입 활용 시 많이 사용되며, 리카로 모든 프로퍼티를 필수로 변경할 수 있다.
- 'Record' 타입은 읽기 전용으로 바꾸는 기능을 제공하며, 초기 할당 이후 값의 변경은 에러를 발생시킨다.

## 2. 📊 레코드 타입 활용하기

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/IeXZo-JXJjc/143.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/IeXZo-JXJjc/143.jpg)

**2.1. 레코드 타입 활용하기**

- '레코드'는 주어진 **키**와 타입으로 구성된 데이터를 다룰 수 있게 해준다.
- 'K'는 키의 타입을 정의하며, 이는 점수와 같은 데이터를 포함할 수 있도록 해준다.
- 예를 들어, 1학년부터 4학년까지의 **점수를 입력**받는 인터페이스를 만들 수 있다.
- 타입을 활용하여 **그레이드**를 키로 사용하고, 1, 2, 3, 4로 정의할 수 있다.
- 이를 통해 코드가 더 간결하고 **깔끔해**질 수 있다.

## 3. 🛠️ 유틸리티 타입의 활용

![https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/IeXZo-JXJjc/318.jpg](https://resource-release.s3.ap-northeast-2.amazonaws.com/thumbnails/IeXZo-JXJjc/318.jpg)

- **K 프로퍼티**만 추출하여 유저 인터페이스에서 특화된 프로퍼티를 사용할 수 있다.
- **익스클루드**는 특정 타입(1에서 8)을 제외하고 남은 프로퍼티를 사용하는 기법이다.
- Remove 함수는 타입에서 특정 프로퍼티를 제거하는 기능을 수행한다.
- **논넥스트**는 널(null) 값을 제외한 새로운 타입을 생성하되, 추가적으로 특정 파인드(find) 값도 함께 제외한다.