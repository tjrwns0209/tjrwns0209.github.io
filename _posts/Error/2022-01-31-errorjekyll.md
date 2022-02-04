---
layout: single
title:  "깃블로그 Error"
comments : ture
categories : [Error]
tags : [jekyll, git-pages, Error]
published: true
toc: true
author_profile: false
sidebar: 
  nav: "docs"
---

# 깃블로그 Error

# 버그 발견(1). 포스팅이 안돼...ㅠ

+ 제대로 파일을 커밋푸쉬했지만, 파일이 포스팅되지 않는 문제가 생겼다... 분명 폴더도 제대로 들어가져 있고, 모든 게 완벽한데... 그래서 구글의 힘을 빌렸다.

<img width="310" alt="2" src="https://user-images.githubusercontent.com/75836426/151710775-277738a8-2c2f-4046-ac78-d09b573b461d.png">

+ 맨 아래에 있는  published: true를 추가!

<img width="482" alt="3" src="https://user-images.githubusercontent.com/75836426/151710806-86b3fdef-9a3f-4d0f-9dd4-2dce9a0063c8.png">

+ 그리고 _config.yml 파일에 future: true를 추가했다.

<img width="456" alt="4" src="https://user-images.githubusercontent.com/75836426/151710816-06becf0f-77be-4ca2-8644-2114348f31a4.png">

+ 딱! 블로그에 정상적으로 포스팅 되었다.... 감사합니다 구글...

# 버그 발견(2). 이미지가 안 뜬다...

+ 경로 확인 모든게 완벽... 다른 거는 다 뜨는데 왜 이거만 안떠... 다시 또 구글링 시작

<img width="721" alt="스크린샷 2022-01-31 02 47 36" src="https://user-images.githubusercontent.com/75836426/151711056-cdc3d33d-7bf8-4799-84a0-95cf01396dd5.png">

+ 꿀팁을 발견했다. 

+ 먼저 Github에 들어가서 ISSUE로 들어가 준다.

<img width="1007" alt="스크린샷 2022-01-31 02 49 30" src="https://user-images.githubusercontent.com/75836426/151711079-587d9764-f76e-4f87-a210-42c67f5339fc.png">

+ 그리고 NEW ISSUE를 누르고 가운데에 이미지를 삽입!

<img width="1382" alt="스크린샷 2022-01-31 02 51 09" src="https://user-images.githubusercontent.com/75836426/151711099-4dc86796-129a-4c94-9d93-a934a06a5171.png">

+ 저 파일경로 그대로 복붙!

<img width="1021" alt="스크린샷 2022-01-31 02 51 27" src="https://user-images.githubusercontent.com/75836426/151711109-919ca764-7e2e-4117-a062-b322dc6b3933.png">

+ 그럼 이미지가 잘 떠요...ㅠㅠ

<img width="677" alt="스크린샷 2022-01-31 02 52 07" src="https://user-images.githubusercontent.com/75836426/151711140-08e5ae91-2362-4f5d-8c4f-6327f490a54f.png">

+ 오늘도 또 한번 구글에 감사합니다...
  + 저 이미지를 폴더에 넣어두고 삭제는 안 해봤는데 혹시 모르니 폴더에는 가지구 있는걸루...
    + 저 만든 ISSUE는 삭제해도 됩니다!