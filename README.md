# react
- @soy22(정소영)

## ch02
### 2.4.1-1
- 컴포넌트에 여러 요소가 있다면 반드시 부모 요소 하나로 감싸야 합니다. 요소 여러 개가 부모 요소 하나에 의하여 감싸져 있지 않기 때문에 오류가 발생했습니다.
### 2.4.1-2
- 리액트 컴포넌트에서 요소 여러 개를 하나의 요소로 감싸 주어 오류를 해결합니다.
### 2.4.1-3
- 여기서 꼭 div 요소를 사용하고 싶지 않을 수도 있습니다. 그런 경우에는 리액트 v16 이상 부터 도입된 Fragment라는 기능을 사용하면 됩니다.
### 2.4.1-4
- Fragment는 다음과 같은 형태로도 표현할 수 있습니다.
### 2.4.2
- JSX 안에서는 자바스크립트 표현식을 쓸 수 있습니다. 자바스크립트 표현식을 작성하려면 JSX 내부에서 코드를 { }로 감싸면 됩니다. 자바스크립트 값을 JSX 안에서 한번 렌더링해 봅시다.
### 2.4.3
- 다른 내용을 렌더링해야 할 때는 JSX 밖에서 if 문을 사용하여 사전에 값을 설정하거나, { } 안에 조건부 연산자를 사용하면 됩니다. 조건부 연산자의 또 다른 이름은 삼항 연산자입니다.
### 2.4.4-1
- null을 렌더링하면 아무것도 보여 주지 않습니다.
### 2.4.4-2
- 더 짧은 코드로 똑같은 작업을 할 수 있습니다. && 연산자를 사용해서 조건부 렌더링을 할 수 있습니다.
### 2.4.5-1
- 리액트 컴포넌트에서는 함수에서 undefined만 반환하여 렌더링하면 오류가 발생합니다.
### 2.4.5-2
- name 값이 undefined일 때 보여 주고 싶은 문구가 있다면 다음과 같이 코드를 작성하면 됩니다.
### 2.4.6-1
- 리액트에서 DOM 요소에 스타일을 적용할 때는 문자열 형태로 넣는 것이 아니라 객체 형태로 넣어 주어야 합니다.
### 2.4.6-2
- 미리 선언하지 않고 바로 style 값을 지정하고 싶다면 다음과 같이 작성하면 됩니다.
### 2.4.7-1
- class 대신 className: src 디렉터리 안에 있는 App.css를 열어서 새 CSS 클래스를 작성
### 2.4.7-2
- App.js 파일에서 상단에 App.css를 불러온 뒤 div 요소에 className 값을 지정
### 2.4.8-1
- input 태그를 닫지 않았을 때 발생하는 오류
### 2.4.8-2
- input 태그를 닫아 오류 해결
### 2.4.8-3
- 태그 사이에 별도의 내용이 들어가지 않는 경우에는 다음과 같이 작성할 수도 있습니다. 이러한 태그를 self-closing 태그라고 부릅니다. 태그를 선언하면서 동시에 닫을 수 있는 태그죠.
### 2.4.9
- 일반 자바스크립트에서 주석을 작성할 때처럼 아무 데나 주석을 작성하면 그 주석은 페이지에 고스란히 나타납니다.
### 2.5.2-1
- 들여쓰기가 제대로 되어 있지 않은 코드
### 2.5.2-2
- 현재 열려 있는 프로젝트의 루트 디렉터리(src, public 디렉터리들이 위치한 곳)에서 .prettierrc라는 파일 생성

## ch03
### 3.1-1
- 2장에서 보았던 App 컴포넌트 - 함수형 컴포넌트
### 3.1-2
- 클래스형 컴포넌트
### 3.2.2
- MyComponent.js 파일을 열고 새 컴포넌트의 코드를 작성(함수형)
### 3.2.3.2
- 모듈 불러오기(import)
### 3.3.2
- App 컴포넌트에서 MyComponent의 props 값을 지정
### 3.3.3
- props 값을 따로 지정하지 않았을 때 보여 줄 기본값을 설정하는 defaultProps
### 3.3.4-1
- 컴포넌트 태그 사이의 내용을 보여 주는 props-children
### 3.3.4-2
- MyComponent 태그 사이에 작성한 리액트라는 문자열을 MyComponent 내부에서 보여 주려면 props.children 값을 보여 주어야 합니다.
### 3.3.5-1
- 작업을 더 편하게 하기 위해 ES6의 비구조화 할당 문법을 사용하여 내부 값을 바로 추출하는 방법. 이렇게 코드를 작성하면 name 값과 children 값을 더 짧은 코드로 사용할 수 있습니다.
### 3.3.5-2
- 함수의 파라미터가 객체라면 그 값을 바로 비구조화해서 사용하는 것이죠. 앞으로 함수형 컴포넌트에서 props를 사용할 때 이렇게 파라미터 부분에서 비구조화 할당 문법을 사용합니다.
### 3.3.6-1
- 컴포넌트의 propTypes를 지정
### 3.3.6-2
- PropTypes를 불러온 후 MyComponent.js 수정. name 값은 무조건 문자열(string) 형태로 전달해야 된다는 것을 의미.
### 3.3.6-3
- App 컴포넌트에서 name 값을 문자열이 아닌 숫자로 전달하면 오류.
### 3.3.6-4
- name 값을 제대로 설정해 주어 오류 해결
### 3.3.6.1-1
- isRequired를 사용하여 필수 propTypes 설정: 아직 favoriteNumber를 설정하지 않았기 때문에 오류
### 3.3.6.1-2
- isRequired를 사용하여 필수 propTypes 설정: MyComponent에게 favoriteNumber 값을 제대로 전달하여 오류 해결
### 3.3.7-1
- 클래스형 컴포넌트에서 props를 사용할 때는 render 함수에서 this.props를 조회하면 됩니다. MyComponent를 다음과 같이 클래스형 컴포넌트로 변환.
### 3.3.7-2
- 클래스형 컴포넌트에서 defaultProps와 propTypes를 설정할 때 class 내부에서 지정하는 방법도 있습니다.
### 3.4.1-1
- 클래스형 컴포넌트의 state: Counter.js 파일을 src 디렉터리에 생성
### 3.4.1-2
- 클래스형 컴포넌트의 state: Counter 컴포넌트를 App에서 불러와 렌더링
### 3.4.1.1
- state 객체 안에 여러 값이 있을 때
### 3.4.1.2
- state를 constructor에서 꺼내기
### 3.4.1.3-1
- this.setState에 객체 대신 함수 인자 전달하기: this.setState를 두 번 사용하는 것임에도 불구하고 버튼을 클릭할 때 숫자가 1씩 더해집니다. this.setState를 사용한다고 해서 state 값이 바로 바뀌지는 않기 때문입니다.
### 3.4.1.3-2
- this.setState에 객체 대신 함수 인자 전달하기: onClick에서 두 번째로 this.setState 함수를 사용할 때는 화살표 함수에서 바로 객체를 반환하도록 했기 때문에 숫자가 2씩 올라갑니다.
### 3.4.1.4
- setState를 사용하여 값을 업데이트하고 난 다음에 특정 작업을 하고 싶을 때는 setState의 두 번째 파라미터로 콜백(callback) 함수를 등록하여 작업을 처리할 수 있습니다.
### 3.4.2.2-1
- 새 컴포넌트를 만들어서 useState를 사용해 보겠습니다. src 디렉터리에 Say.js라는 파일을 생성.
### 3.4.2.2-2
- Say 컴포넌트를 App에서 렌더링
### 3.4.2.3
- 한 컴포넌트에서 useState 여러 번 사용하기

## ch04
### 4.2.1.1
- 새 클래스형 컴포넌트 작성. src 디렉터리 내부에 EventPractice.js 파일 만들기.
### 4.2.1.2
- App.js에서 EventPractice 렌더링
### 4.2.2.1-1
- EventPractice 컴포넌트에 input 요소를 렌더링하는 코드와 해당 요소에 onChange 이벤트를 설정하는 코드를 작성
### 4.2.2.1-2
- 비동기적으로 이벤트 객체를 참조할 일이 있다면 e.persist() 함수를 호출해 주어야 합니다. 예를 들어 onChange 이벤트가 발생할 때, 앞으로 변할 인풋 값인 e.target.value를 콘솔에 기록해 보겠습니다.
### 4.2.2.2
- state에 input 값 담기
### 4.2.2.3
- 버튼을 누를 때 comment 값을 공백으로 설정
### 4.2.3.1
- 앞서 onChange와 onClick에 전달한 함수를 따로 빼내서 컴포넌트 임의 메서드를 만들어 보겠습니다.-기본 방식
### 4.2.3.2
- Property Initializer Syntax를 사용한 메서드 작성
### 4.2.4
- input 여러 개 다루기 
### 4.2.5
- onKeyPress 이벤트 핸들링: 키를 눌렀을 때 발생하는 KeyPress 이벤트를 처리하는 방법
### 4.3-1
- 위의 작업들을 함수형 컴포넌트로 구현해 보기
### 4.3-2
- 이번에는 useState를 통해 사용하는 상태에 문자열이 아닌 객체를 넣어 보겠습니다.
