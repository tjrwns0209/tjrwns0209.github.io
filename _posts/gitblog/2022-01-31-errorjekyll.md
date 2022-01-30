---
layout: single
title:  "깃블로그 Error"
comments : ture
categories : [jekyll, Error]
tags : [jekyll, git-pages, Error]
published: true
---

## 블로그를 운영하면서 버그를 발견할 때마다 계속 업데이트 예정

# 버그 발견(1). 포스팅이 안돼...ㅠ

+ 제대로 파일을 커밋푸쉬했지만, 파일이 포스팅되지 않는 문제가 생겼다... 분명 폴더도 제대로 들어가져 있고, 모든 게 완벽한데... 그래서 구글의 힘을 빌렸다.

<img src="../../assets/img/스크린샷 2022-01-31 02.09.18.png">

+ 맨 아래에 있는  published: true를 추가!

<img src="../../assets/img/스크린샷 2022-01-31 02.10.55.png">

+ 그리고 _config.yml 파일에 future: true를 추가했다.

<img src="../../assets/img/스크린샷 2022-01-31 02.11.46.png">

+ 딱! 블로그에 정상적으로 포스팅 되었다.... 감사합니다 구글...