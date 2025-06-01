## Local Storage

유효기간이 없이 저장되며 제거하기 위한 작업(Javascript를 이용한 제거 혹은 브라우저 캐시)으로 제거된다.

### 예시

```js
localStorage.setItem("key", "저장하고 싶은 데이터");

console.log(localStorage.getItem("key")); // 저장하고 싶은 데이터
```
