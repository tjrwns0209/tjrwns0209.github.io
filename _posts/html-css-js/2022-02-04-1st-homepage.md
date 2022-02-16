---
layout: single
title:  "홈페이지 만들어보기"
date: 2022-02-11 05:00:00  +0900
last_modified_at:  #마지막 수정 시간 적기
comments : ture
categories : [html]
tags : [html, css, javascript, FTP, homepage]
published: true
toc: true 
author_profile: false
sidebar: 
  nav: "docs"
---


# 홈페이지 기록

+ 학교 관련해서 정보들이나 시간표, 일정... 등을 한 번에 모아두기 위해 만들기 시작

<div class="notice--danger">
  <h4>변경 공지</h4>
  <ul>
    <li></li>
  </ul>
</div>

# 시작

+ 폴더를 생성하고 index.html 파일을 만들어줌.

+ 참고 

![스크린샷 2022-02-11 05 30 22](https://user-images.githubusercontent.com/75836426/153491427-e9ae6843-178a-4d50-8468-f8c931124287.png)

css나 js 등 이런 파일은 assets 폴더를 만들어서 넣어주면 깔끔하답니다.

+ index.html 파일 내에서 `!` 를 입력하고 엔터하면 

![스크린샷 2022-02-11 05 22 42](https://user-images.githubusercontent.com/75836426/153490364-1c1c04da-c6d3-49f5-a766-cb4a9ed673dd.png)

이런식으로 자동으로 작성됨.

## 2022-02-11 틀 잡기

![스크린샷 2022-02-11 05 26 28](https://user-images.githubusercontent.com/75836426/153490872-e05ae9fd-2ef7-4f2b-aa59-5685854c6429.png)

먼저 이런식으로 빠르게 틀만 잡아줌.

### 사이드바 완성

![스크린샷 2022-02-11 05 31 46](https://user-images.githubusercontent.com/75836426/153491589-c211b0a3-dafc-4fff-b27c-20519f12e3d3.png)

![스크린샷 2022-02-11 05 31 56](https://user-images.githubusercontent.com/75836426/153491605-731ac38b-dd3c-403a-96b2-b9857918f316.png)

이런식으로 열기 닫히는 사이드바를 완성함

```javascript
const open = document.querySelector('.side-bar-open-btn');
const close = document.querySelector('.side-bar-close-btn');
const sideBar = document.querySelector('.side-bar-contents');

//open
open.addEventListener('click', function(){
  sideBar.style.left = "0";
})

//close
close.addEventListener('click', function(){
  sideBar.style.left = "-600px";
})
```

+ const open => 웹 페이지에서 side-bar-open-btn 이라는 클래스 명을 찾음   
밑에 2개도 다 똑같음

+ addEventListener를 사용해서 클릭했을 때 sideBar의 스타일이 변경되도록 해줌.

## 2022-02-12 index.html을 깔끔하게 해줌

+ index.html의 내용물이 점점 쌓여가자 너무 복잡해짐

+ 구글링을 통해 html을 include할 방법을 찾음

```javascript
$(document).ready(function wrapper() {
  $("나타낼 위치").load("html의 경로");
})
```

![스크린샷 2022-02-12 04 39 16](https://user-images.githubusercontent.com/75836426/153658320-471ba029-6f42-40da-bc64-0bbf231340f7.png)

index의 내용을 담아줄 파일들을 생성함

![스크린샷 2022-02-12 04 36 32](https://user-images.githubusercontent.com/75836426/153658030-ad607709-a85a-41d3-86cd-2dd86c781ee5.png)

덕분에 index.html이 엄청 깔끔해짐...ㅠ 이렇게 알아가는 맛에 코딩하고, 개운함에 코딩하지...ㅎ

+ 근데 스크립트 적용이 약간 이상함 index.html에 적용되어 있는 스크립트가 적용되지 않아서 새로 만든 파일들에 직접 스크립트를 호출해서 해결하긴 했는데... 이건 좀 이해가 안되네요...