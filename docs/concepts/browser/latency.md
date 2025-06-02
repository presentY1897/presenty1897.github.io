---
layout: page
title: Latency
parent: Browser
permalink: /docs/concepts/browser/latency/
---

# Latency

대기 시간은 데이터가 도착하는 데 걸리는 시간을 의미한다. 웹 페이지의 성능에 영향을 주는 요소 중에 하나로 대기 시간을 줄여 성능을 최적화 할 수 있다. 웹 페이지는 접속 과정^[1](/docs/concepts/browser/populating-the-page/)에서 DNS 조회, TCP handshake, 보안 TLS를 거치고 웹 페이지를 구성하는 HTML, CSS, Javascript나 font, image 등의 요소를 요청한다. 이 과정에서 각각 대기 시간이 발생한다.

---

#### 참조

1. [Mozilla, Understanding latency](https://developer.mozilla.org/en-US/docs/Web/Performance/Guides/Understanding_latency)
