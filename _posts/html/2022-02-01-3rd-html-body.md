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
    <li>작성 완료(22-02-02-19:44)</li>
  </ul>
</div>

# HTML의 body에 포함되는 태그

+ 주석 사용법
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
+ `<input>` + `<select>`
+ `<button>`
+ `<img>`
+ `<table>`
+ `<iframe>`
+ `<strong>` + `<b>` + `<i>`
+ 구역을 나누는 태그(header, footer...)

...등 굉장히 많아요... 천천히 하나하나 같이 배워봐요!

앞으로 html 코드들을 보여드릴 건데 다른 건 다 신경쓰지 마시고, body태그 안에만 집중해 주세요!!

# 주석 사용법

+ 모든 주석은 입력후   
cmd + / (mac)   
con + / (win)   
자동으로 주석처리됩니다.

+ html의 주석은

```
<!-- content -->
```

이렇게 작성합니다.

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

# `<input>` 태그 + `<select>` 태그

+ 이 태그의 type에 따라서 사용되는 용도가 달라집니다.   
input의 type에 대해서 알아볼게요

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
	id : <input type="text"> <br>
	password : <input type="password"> <br>
	<input type="radio">코딩하기 <br>
	<input type="radio" checked>잠자기 <br>
	<input type="checkbox">놀기 <br>
	<input type="checkbox" checked>밥먹기 <br>
	<input type="button" value="im btn"> <br>
	<input type="submit" value="sign up"> <br>
	<input type="reset" value="reset"> <br>
	<input type="image" src="경로"> <br>
	<input type="file"> <br>
	<select>
		<option>select</option>
		<option>1</option>
		<option>2</option>
		<option>3</option>
		<option>4</option>
		<option>5</option>
	</select>
    <script src="script.js"></script>
  </body>
</html>
```
+ 위의 내용은 이렇게 보여요!

<img width="280" alt="스크린샷 2022-02-02 14 54 07" src="https://user-images.githubusercontent.com/75836426/152100550-43140971-3ba5-4c06-8f95-f5d89672a1d5.png">

# `<button>` 태그

+ input 태그에도 button이라는 type이 존재합니다. 하지만 input과는 달리 button은 자유롭습니다. input은 css를 통해 이미지를 삽입하거나 할 수 있지만 button는 하위에 img태그를 이용해 바로 이미지를 삽입할 수 있습니다. 

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
	  <button>
		  <img src="https://user-images.githubusercontent.com/75836426/152100550-43140971-3ba5-4c06-8f95-f5d89672a1d5.png" width="100" onclick="alert('멍!')">
	  </button>
    <script src="script.js"></script>
  </body>
</html>
```

# `<img>` 태그

+ 이미지를 삽일할 수 있는 태그

```html
<img src="경로" alt="강아지 사진" width="100">
```

+ 위의 내용은 이렇게 보여요!

<button>
  <img src="https://user-images.githubusercontent.com/75836426/151710514-4b5e5892-38dd-47dd-b944-adeab9d2ca78.jpg" width="100" onclick="alert('멍!')">
</button>
나를 눌러바!

# `<table>` 태그

```html
<table>
    <thead>
        <tr>
            <th>Table입니다.</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>안녕하세요</td>
            <td>반갑습니다.</td>
        </tr>
    </tbody>
</table>
```

+ 위의 내용은 이렇게 보여요!

<table>
    <thead>
        <tr>
            <th>Table입니다.</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>안녕하세요</td>
            <td>반갑습니다.</td>
        </tr>
    </tbody>
</table>

## `<table>` 디자인

+ colspan : 가로 합병
+ rowspan : 세로 합병
+ border : 테두리
+ bordercolor : 테두리의 색
+ width : 가로 크기
+ height : 세로 크기
+ align : 정렬
+ bgcolor : 배경색

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
<table border="1" align="center" bordercolor="blue">
  <tr>
    <th colspan="2">Table입니다.</th>
  </tr>
  <tr>
    <td>안녕하세요</td>
    <td>반갑습니다.</td>
  </tr>
</table>
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 보여요!

<img width="753" alt="스크린샷 2022-02-02 15 40 30" src="https://user-images.githubusercontent.com/75836426/152106106-6170f9b8-41c2-4eec-82da-69fb8318424c.png">

# `<iframe>` 태그

+ 웹 페이지 안에 다른 하나의 웹 페이지를 삽입하는 태그

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
<iframe src="경로" width="100%"></iframe>
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 보여요!

<iframe src="경로" width="100%"></iframe>

# `<strong>` 태그 + `<b>` 태그 + `<i>` 태그

+ strong 태그는 글자를 강조해주고 웹에게 이 부분은 굉장히 중요한 부분이라고 알려줍니다. 하지만 b 태그는 그냥 굵게 강조표시만 해줍니다.

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
	  <b>나는 blod!</b> <br>
	  <strong>나는 strong!</strong>
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 보여요!

<b>나는 blod!</b> <br>
<strong>나는 strong!</strong>

보기엔 똑같이 보이지만 음성인식기능을 이용하면 strong 태그를 이용한 부분은 강조해서 읽어줍니다. 

## `<i>` 태그

+ 글자를 기울여주는 태그입니다. 

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
	  <i>나는 italic!</i>
    <script src="script.js"></script>
  </body>
</html>
```

+ 위의 내용은 이렇게 나타나요!

<i>나는 italic!</i>

# `<nav>` 태그

+ nav 태그는 목차나 메뉴 등의 링크들을 보여줄 때 자주 사용됩니다. 

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
	  <nav>
		  <ul>
			  <li><a href="#">nav1</a></li>
			  <li><a href="#">nav1</a></li>
			  <li><a href="#">nav1</a></li>
		  </ul>
	  </nav>
    <script src="script.js"></script>
  </body>
</html>
```
+ 위의 내용은 이렇게 보여요!

> <nav>
>   <ul>
>     <li><a href="#">nav1</a></li>
>     <li><a href="#">nav1</a></li>
>     <li><a href="#">nav1</a></li>
>   </ul>
> </nav>

# 구역을 나누는 태그

+ `<nav>` : 메뉴
+ `<header>` : 머리글
+ `<section>` : 구역을 나누는 태그
+ `<article>` : 본문
+ `<aside>` : 사이드 메뉴
+ `<footer>` : 저작권 등을 표시하는 하단 부분

이 부분은 사진으로 설명드릴께요

+ 네이버 웨일 기능인 부분 캡처를 통해서 네이버 페이지를 한 번 살펴볼께요.

+ `<header>`

<img width="1440" alt="스크린샷 2022-02-02 19 34 06" src="https://user-images.githubusercontent.com/75836426/152137901-e69a9352-03e8-4722-980e-5db5a2839d83.png">

+ `<nav>`

<img width="1440" alt="스크린샷 2022-02-02 19 34 15" src="https://user-images.githubusercontent.com/75836426/152138014-ed2a3f42-04ba-4900-b12f-be5cd2cc4ef3.png">

+ `<section>`

<img width="1440" alt="스크린샷 2022-02-02 19 34 19" src="https://user-images.githubusercontent.com/75836426/152138155-9b717197-2bca-410c-a5c8-11c31792f056.png">

+ `<article>`

<img width="1440" alt="스크린샷 2022-02-02 19 34 22" src="https://user-images.githubusercontent.com/75836426/152138299-1dd26729-d604-4c73-9be9-9e66fc282831.png">

+ `<aside>`

<img width="1440" alt="스크린샷 2022-02-02 19 34 45" src="https://user-images.githubusercontent.com/75836426/152138362-b930eeb3-7007-4007-9c78-b27d1118a037.png">

+ `<footer>`

<img width="1440" alt="스크린샷 2022-02-02 19 35 04" src="https://user-images.githubusercontent.com/75836426/152138455-b351361f-14ed-47c2-8e25-00257e9d9658.png">

