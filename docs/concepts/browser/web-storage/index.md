---
layout: page
title: Web Storage
parent: Browser
permalink: /docs/concepts/browser/web-storage/
---

# Web Storage

[쿠키](/docs/concepts/browser/cookie/)와 같이 브라우저에서 데이터를 저장하는 방법이다. 차이점은 쿠키가 4KB의 데이터만 저장할 수 있는 반면에 웹 스토리지는 5MB 까지의 데이터를 저장할 수 있다는 점과 쿠키는 서버에 요청시에 도메인과 일치하는 모든 쿠키를 전송하지만 웹 스토리지는 그렇지 않다는 점이 있다.

{% include_relative local-storage.md %}

{% include_relative session-storage.md %}

---

#### 참조

1. [Mozilla, Web Storage API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API)

1. [개발 블로그, 웹 스토리지의 특성과 사용법](https://untitledtblog.tistory.com/47)
