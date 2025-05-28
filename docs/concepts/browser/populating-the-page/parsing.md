### 구문 분석(Parsing)

구문 분석은 데이터를 DOM이나 CSSOM으로 바꾸는 과정이다. 결과는 렌더러가 화면을 그리는 데 사용한다.

1. DOM 트리 구축(Building the DOM tree)
1. Preload Scanner
1. CSSOM 구축(Building the CSSOM)
1. Javascript Compilation
1. 접근성 트리 구축(Building the Accessibility Tree)

DOM tree는 HTML을 분석한 결과물을 말한다. HTML의 구문 분석은 토큰화와 트리 생성을 수행한다. 최종적으로 DOM tree는 태그 간의 관계와 계층으로 구성된다. 구문 분석기가 이미지나 css파일의 참조를 확인하면 데이터를 요청하고 분석을 계속 진행한다. 하지만 `async`나 `defer` 설정이 되어 있지 않은 `<script>` 태그는 구문 분석을 중지하고 데이터를 받을 때까지 기다린다.

프리로드 스캐너는 브라우저가 DOM tree를 생성하는 동안 백그라운드에서 css, javascript, web-font와 같은 자원을 요청한다. 그래서 구문 분석기가 해당 자원을 요청해야하는 지점에 도달했을 때, 이미 프리로드 스캐너가 요청을 한 뒤이다.

DOM tree와 마찬가지로 CSS를 처리하여 CSSOM 트리를 생성한다. CSSOM을 만드는 시간은 매우 짧아 성능을 최적화하기에는 적합하지 않다.

Javascript 파일도 다운로드 후에 처리를 위해 compile을 진행한다.

브라우저는 접근성 트리도 생성한다.
