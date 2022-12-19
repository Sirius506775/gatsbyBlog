	#react

**index.js** 파일이 가장 먼저 실행되는 파일이다.

`import ReactDOM from 'react-dom/client';` 
React-dom이라는 패키지로부터 reactDOM Object를 가져온다

pakage.json를 살펴보면 
로컬에 설치한 dependencies를 확인할 수 있다. 

![[Pasted image 20221219150604.png]]

엄밀히 말하면 별개의 패키지로 나누어 각기 다른 역할을 하지만 두 가지 React 라이브러리에 의존한다. 

index.js처럼 말이다.
해당 라이브러리가 제공하는 기능을 사용할 수 있는 것이다.

이게 현대 JavaScript의 일반적인 작동 방식이다. 

React-dom이라는 패키지로부터 reactDOM Object를 가져와서 creatRoot 메소드를 호출한다. 

![[Pasted image 20221219150631.png]]
이로 인해 주요 엔트리 포인트가 생성된다. 

리액트로 구축될 UI에 대한 주요 hook을 말한다. 

### createRoot 메소드의 역할 :

리액트로 구축할 UI를 리액프 어플리케이션이 불러온 웹페이지 상에서 어디에 배치해야하는지 리액트에게 알려주는 메소드이다. 
이 메소드로 인해 public 폴더에 있는 index.html로 이동하게된다. 

![[Pasted image 20221219150641.png]]

단일 html파일로 브라우저가 불러오는 파일이다. 

리액트 어플리케이션 전체에서 사용하는 유일한 html 파일이다. 
단일 페이지 어플리케이션, SPA라고 불리는 부분이다.

리액트로 다루는 웹페이지와 UI에서 일어나는 모든 변경사항들을 다룬다. 

엔트리 포인트인 이 단일 HTML 파일은 React가 주도하는 UI가 렌더링되야하는 위치이다. 

![[Pasted image 20221219150648.png]]

우리는 이 div태그에 react로 구축할 UI를 추가한다. 

React를 기반으로 하는 사용자 인터페이스가 렌더링되어야 하는 건 이 div 태그입니다
```javascript
import ReactDOM from 'react-dom/client';

  

import './index.css';

import App from './App';

  
//root 객체를 상수나 변수로 저장
const root = ReactDOM.createRoot(document.getElementById('root')); //메인 react 어플리케이션이 렌더링되는 부분이다.
//root라는 id를 갖고 있는 dom이 루트라는 것을 react에게 알려준다.


root.render(<App />);
//root객체에서 render메소드를 호출
```

그 다음, root객체에서 render메소드를 호출해서 이 div 태그에 뭘 렌더링해야 하는지 알린다.

그 다음 ReactDOM에게 렌더링하고 싶은 게 있다고 알린다. 

div 태그에 들어갈 콘텐츠는 App이다.
`import App from './App';` 


