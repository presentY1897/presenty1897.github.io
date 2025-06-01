## Session Storage

Domain에 따라서 독립적으로 데이터를 저장하고 세션이 열려있는 동안(브라우저가 닫히기 전까지)만 저장된다. 저장 공간은 최대 5MB까지 가능하다.

### 예시

```js
sessionStorage.setItem("key", "저장하고 싶은 데이터");

console.log(sessionStorage.getItem("key")); // 저장하고 싶은 데이터
```
