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

<img width="310" alt="2" src="https://user-images.githubusercontent.com/75836426/151710775-277738a8-2c2f-4046-ac78-d09b573b461d.png">

+ 맨 아래에 있는  published: true를 추가!

<img width="482" alt="3" src="https://user-images.githubusercontent.com/75836426/151710806-86b3fdef-9a3f-4d0f-9dd4-2dce9a0063c8.png">

+ 그리고 _config.yml 파일에 future: true를 추가했다.

<img width="456" alt="4" src="https://user-images.githubusercontent.com/75836426/151710816-06becf0f-77be-4ca2-8644-2114348f31a4.png">

+ 딱! 블로그에 정상적으로 포스팅 되었다.... 감사합니다 구글...