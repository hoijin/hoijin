---
title: "Nodejs 시작"
date: 2019-09-15 20:03:28 -0400
categories: Nodejs
link: https://www.w3schools.com/nodejs/
---

오늘은 NodeJS로 Hello world! 출력을 목표로 시작해보자.

1. hello.js 파일 생성

Atom에서 hello.js 파일을 생성하고 아래와 같은 코드를 입력해주고

<pre><code>var http = require('http');

http.createServer(function (req, res) {
  res.writeHead(200, {'Content-Type': 'text/html'});
  res.end('Hello World!');
}).listen(8000);
</code></pre>

2. 웹 브라우저에서 Hello World! 출력

명령 프롬프트에 node hello.js를 입력해서 로컬 서버를 구동 시키고

웹 페이지에 localhost:8000 을 입력해주면 끝!


+ 추가 

공부 목적인 만큼 위 코드를 왜 사용하고 Nodejs는 무엇인지에 대해 알아봐야겠다.

0. NodeJS

NodeJS는 자바스크립트를 이용한 비동기 IO 및 Single-Thread 기반으로 동작하는 서버라고 한다.

이 말은 학습하면서 차차 알아 가기로 해야겠다. (다음에 글을 쓰게 된다면 여기에 링크를 걸어야겠다.)

1. 모듈

모듈은 자바스크립트로 된 라이브러리이다. 

기본으로 설치가 필요 없는 빌트인 모듈이 존재하고 이 모듈을 사용하기 위해서는 require() 이 함수를 사용해야한다고 한다.

개인으로 모듈을 만들 수도 있고 만든 모듈을 사용하기 위해서는 모듈의 파일의 경로를 require('path') 이와같이 작성하면 된다.

2. Http 모듈

Http 모듈은 위에서 설명한 빌트인 모듈이다.

이 모듈은 http 프로토콜을 제공해준다.

이 모듈에 대해 자세한 내용은 아래 출처에 있다.

한 건 없지만 오늘은 여기까지...!


출처 : [https://www.w3schools.com/nodejs/](https://www.w3schools.com/nodejs/) 










