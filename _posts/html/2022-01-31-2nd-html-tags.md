---
layout: single
title:  "HTML Tags"
comments : ture
categories : [html]
tags : [html, html tag]
published: true
---

# 이번에는 HTML의 head에 포함되는 태그들에 대해서 알아볼게요. 

+ 먼저 `<head>`태그 안에는 `<link>, <meta>, <title>, <style>, <script>` 등이 가장 대표적으로 쓰이게 됩니다. (제가 만들면서도 이게 가장 많이 쓰였어요..ㅎㅎ) 이제 각각 무슨 역할을 하는지 알아볼게요.

# `<link>`

외부의 파일을 가져올 때 사용되게 되는데요.   
에시로 css를 불러올때를 보여드릴게요.

```html
<link href="경로", rel="stylesheet" type="text/css"/>
```

이렇게 쓰이게 됩니다. 이론적인 부분은 빼고, css를 불러올 때는 저런식으로 작성하시면 됩니다. 

# `<meta>` 

이 태그는 문서를 설명해주는 태그이고,   
누가 만들었는지, 키워드가 무엇인지, 언어는 뭔지 등 이런 정보들을 담고 있습니다.    
예시를 보여드릴께요.

```html
<meta charset="UTF-8"> // 언어설정
```

문자 인코딩 방식을 UTF-8로 하라는 뜻입니다. 

# `<title>`

<img width="183" alt="스크린샷 2022-01-31 14 14 13" src="https://user-images.githubusercontent.com/75836426/151742357-4212503d-0d16-4da4-9a4b-c8a012baa758.png">

이처럼 탭에 나타나는 제목으로 나타납니다. 

```html
<title>제목입니다.</title>
```

이런식으로 작성합니다. 

+ 네 번째로 `<style>` 입니다. 이 태그는 따로 css파일을 만들지 않고 index.html에서 직접 css를 작성할 수 있는 태그입니다. 

```html
<style>
  .title {
    ...
  }
</style>
```

이런식으로 index.html 내에서 css를 작성할 수 있습니다.

# `<script>` 

저는 `<head>`에 작성되는 `<script>`에는 외부 스크립트 파일을 가져올 때 사용합니다. 그 외에 제가 작성하는 스크립트 파일은 `<body>` 태그 맨 아래에 작성합니다. 이렇게 사용하는 이유는 구글링을 하면서 스크립트를 `<body>` 태그 맨 아래에 적용하는 것이 가장 빠르다고 하여서 이렇게 작성하게 되었습니다. 왜냐하면 html은 js를 만나게 되면 일단 js를 먼저 읽기 때문에 멈추게 됩니다. 그리고 다 읽게되면 다시 html파일을 다시 읽어옵니다.  
(대충 이런식으로 이해 했어요...)

```html
<script src="경로"></script>
```

스크립트는 이런식으로 불러오시면 되고, 

```html
<script>
  function hihi() {
    ...
  }
</script>
```

이런식으로 바로 스크립트를 작성할 수도 있습니다. 

## `<head>` 태그...

태그는 제가 웹을 만들면서 그렇게 신경을 많이 쓰는 부분은 아니여서 그런지 생각보다 각각의 태그들에 대해서 미흡한 부분들이 좀 있네요. 이번 포스팅을 계기로 `<head>` 태그에 포함되는 태그들이 각각 어떠한 역할을 하는지 알아볼 수 있어 좋은 시간이었네요:)