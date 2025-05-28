---
layout: page
permalink: /docs/concepts/browser/dns-lookup/
---

# DNS Lookup

웹 페이지에 접속할 때 페이지의 주소를 찾는 과정이다. 예를 들어 `google.com`을 접속하면 웹 페이지가 위치한 서버의 IP인 `142.251.12.101`를 찾는다.

처음으로 접속하는 주소라면 DNS lookup을 수행한다. 브라우저에서 DNS lookup을 요청하면 Name Server에 접근하여 IP 주소를 반환받는다. 반환된 결과를 캐시하여 다시 같은 주소로 접속할 때는 저장한 IP 주소를 사용하여 Name Server에서 조회하는 시간을 단축한다.
