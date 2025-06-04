---
layout: page
title: React state
parent: React
permalink: /docs/concepts/react/state/
---

react는 state를 이용한 선언적 방식의 UI를 추천한다. 선언적 방식은 명령적 방식과 대조적으로 명령적은 어떤 행동을 하면 어떤 효과가 발생하는 지를 정의하는 반면, 선언적 방식은 어떤 state에 따라 표현하는 것을 정의한다.

로그인 페이지를 예로 들어 id, password 입력창과 접속 button이 있는 페이지를 가정한다.

```html
<div>
  <p>ID</p>
  <input id="id-input" />
  <p>PASSWORD</p>
  <input id="id-password" />
  <button id="submit-button">submit</button>
</div>
```

일반적으로 로그인 페이지의 스펙에는 id와 password가 모두 입력하면 버튼이 활성화되고 서버에 로그인을 시도하면 버튼이 비활성화되는 스펙을 가정할 수 있다.

명령적 방식이라면 id와 password input에 값이 입력되면 버튼을 활성화하고 버튼을 누르면 다시 서버에서 응답이 올때까지 비활성화하는 식으로 접근한다.

선언적 방식은 버튼이 활성화/비활성화 state를 가지고 그에 따른 결과만 대응하게 하고, input에서 변화가 발생하면 state를 알맞게 변형하는 방식으로 접근한다.
