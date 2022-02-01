---
layout: single
title:  "HTML Tags <body>"
comments : ture
categories : [html]
tags : [html, html tag]
published: true
toc: true 
author_profile: false
sidebar: 
  nav: "docs"
---


# HTML 태그

이번 포스팅은 굉장히 길어지겠네요...ㅎ

[replit](https://replit.com){: .btn .btn--danger} 클릭!

따라 코딩하실 때 저거 이용해 보세요. 좋아요...! 편리합니당.

html 외에도 많은 언어 지원하니까 참고하세요!!

<div class="notice--danger">
  <h4>변경 공지</h4>
  <ul>
    <li>작성중...!</li>
  </ul>
</div>

# HTML의 body에 포함되는 태그

+ `<br>` 
+ `<div>`
  + style
  + class, id 차이점
+ `<span>`
+ `<p>`
+ `<a>`
+ `<h>`
+ `<ul>`
+ `<li>`
+ `<ol>`
+ `<input>`
+ `<img>`
+ `<table>`
+ `<form>`
+ `<iframe>`
+ `<nav>`
+ `<strong>`
+ `<fotter>`
+ `<header>`
+ `<button>`
+ `<i>`
+ `<b>`
+ `<section>`
+ `<article>`
+ `<aside>`
+ 주석 사용법

...등 굉장히 많아요... 천천히 하나하나 같이 배워봐요!

앞으로 html 코드들을 보여드릴 건데 다른 건 다 신경쓰지 마시고, body태그 안에만 집중해 주세요!!

# `<br>`태그
+ 줄을 바꿔주는 태그 입니다. 

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>replit</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    Hello world1
    Hello world2
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 나타나요!

```
Hello world1 Hello world2
```

분명 줄은 바뀌었지만 적용이 되지 않았습니다. 이때 사용하는 태그가 `<br>`태그 입니다. 

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>replit</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    Hello world1
    <br>
    Hello world2
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 보여요!

```
Hello world1   
Hello world2
```

줄바꿈이 적용되었죠?? 이게 `<br>` 태그입니다. 

# `<div>` 태그
+ 이 태그는 그냥 내용을 따로 묶어낼 때 사용되는 태그입니다. 굉장히 많이 쓰이는 태그에요.

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>replit</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    안녕
    <div>
      안녕
    </div>
    안녕
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 보여요!

```
안녕
안녕 
안녕
```

+ div 태그에 class라는 걸 부여할 수도 있고, style을 부여할 수도 있습니다. 

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>replit</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <div class="className">
      안녕 나는 division이라구해
    </div>
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 보여요!

```
안녕 나는 division이라구해 
```

+ 저 class를 이용해서 각각 css를 적용할 수도 있습니다. 

## class와 id의 차이점.
+ class는 한 요소에 여러개의 클래스 명이 적용될 수 있지만, id는 한 요소에 하나의 한 id만 적용 가능하고, css를 부여할 때 순위는 class보다는 id가 더 우선적으로 적용됩니다!   
class = 하나 이상!!   
id = 무조건 하나!!

# `<span></span>` 태그

+ span 태그는 기본적으로 div 태그와 다르게 inline 요소를 가지고 있습니다. 

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>replit</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
    <div class="className1" style="background-color: red;">
      안녕 나는 division이라구해
    </div>
	<span class="className2" style="background-color: blue;">
		안녕 나는 span이라구해
	</span>
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 보여요!

```
안녕 나는 division이라구해   
안녕 나는 span이라구해
```

+ inline이 뭐에요...?

<img width="758" alt="스크린샷 2022-02-02 01 08 48" src="https://user-images.githubusercontent.com/75836426/152005402-da9b1f63-1c85-4767-8862-60641f137a4a.png">

+ div 태그와는 다르게 span 태그는 딱 맞게 배경이 설정이 되었죠. 그게 inline이에요!   
div와 span은 그 차이를 가지고 있어요!

# `<p></p>` 태그

+ `<p></p>` 태그는 문단을 만들어줄 때 사용되는 태그입니다. 

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>replit</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
	  <p>
		  안녕! 나는 paragraph야!
	  </p>
	  <p>
		  안녕! 나는 paragraph야!
	  </p>
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 나타나요!!

```
안녕! 나는 paragraph야!

안녕! 나는 paragraph야!
```

+ 앞의 div 태그와 span태그와의 차이점이 느껴지시나요??

+ 위의 태그들과는 다르게 위쪽과 아래쪽에 약간의 여백이 추가됐어요.

# `<a>` 태그

+ `<a>`태그는 다른 페이지의 링크를 걸어줄 때 사용됩니다. 

```html
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>replit</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
	  <a href="https://google.co.kr">google</a>
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 보여요!

<a href="https://google.co.kr">google</a>

+ 또한 a태그에는 target이라는 속성이 존재합니다. 

+ _blank : 링크를 새 탭으로 열어줍니다.   
_self : 현재 페이지에 링크를 열어줍니다. (기본값!)

```html
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>replit</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
	  <a href="https://google.co.kr" target="_blank">google</a>
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 보여요!

<a href="https://google.co.kr" target="_blank">google</a>

+ 처음과는 다르게 새 탭에서 링크가 열리는 것을 확인할 수 있어요.

# `<h>` 태그

+ h태그는 markdown의 #과 같은 역할을 하는 태그에요.

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>replit</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
	  <h1>h1</h1>
	  <h2>h2</h2>
	  <h3>h3</h3>
	  <h4>h4</h4>
	  <h5>h5</h5>
	  <h6>h6</h6>
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 보여요!

<h1>h1</h1>
<h2>h2</h2>
<h3>h3</h3>
<h4>h4</h4>
<h5>h5</h5>
<h6>h6</h6>

# `<ul>`, `<li>`, `<ol>` 태그

+ 목록을 나타내주는 태그입니다. 

```html
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>replit</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>
  <body>
	  <ul>
		  <li>ul + li</li>
	  </ul>
	  <ol>
		  <li>ol + li</li>
	  </ol>
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 보여요!

> <ul>
> <li>ul + li</li>
> </ul>
> <ol>
> <li>ol + li</li>
> </ol>