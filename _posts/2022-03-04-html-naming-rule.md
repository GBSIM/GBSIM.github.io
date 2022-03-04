---
layout: single
title: "HTML style guide"
category: Coding
tag: [HTML,웹개발]
toc: true
---

웹개발에 있어서 웹의 전반적인 형태를 만들어주는 가장 기초적인 부분이 HTML과 CCS에요.

오늘은 HTML의 style guide에 대해서 다뤄보겠습니다~! 본 포스팅의 stye guide는 <strong>w3schools.com</strong>의 HTML style guide를 기반으로 작성되었어요.
<br>
<br>

# 소문자를 사용해주세요.

HTML 코딩 시에는 소문자만을 사용하세요! 대문자를 이용해서 코딩하더라도 정상적으로 동작하겠지만, 아래 이유들 때문에 소문자 사용을 추천드려요.

- 대문자와 소문자를 섞어 쓸 경우 코드를 읽기 불편해요.
- 개발자들은 대부분 코딩 시 소문자를 사용해요.
- 소문자가 코딩하기 훨씬 쉬워요.

<strong>아래처럼 소문자만을 사용해주세요! </strong>

```html
<body>
<p> This is a pragraph.</p>
</body>
```
<br>


# 모든 HTML element를 닫아주세요.

모든 HTML element를 닫는 형태로 코딩하지 않아도 정상 동작해요. 하지만, 통일성을 위해서 모든 element는 닫는 형태로 코딩해주세요.

```html
<section>
    <p>This is a paragraph.</p>
    <p>This is a paragraph.</p>
</section>
```
<br>

# Attribute에는 소문자를 사용해주세요.

HTML element들의 attribute에는 소문자만을 사용해주세요. 이유는 guide 01과 같아요!

```html
<a href="https://gbsim.github.io">Visit Gyubin's blog</a>
```
<br>

# 모든 attribute 값에는 큰따옴표를 붙여주세요.

Attribute의 값에는 문자를 그대로 집어넣기보다는 큰따옴표를 꼭 사용해주세요!

```html
<div class="header"></div>
```
<br>

# 이미지를 넣을 때는 alt, width, height 속성값을 넣어주세요.

이미지를 넣을 때는 위의 세 attribute 값을 꼭 넣어주세요. 이미지가 잘 못 표시되거나 의도하지 않은 크기로 표시되는 것을 최대한 막을 수 있어요!

```html
<img src="pokemon.gif" alt="HTML5" style="width:200px;height:200px;">
```
<br>
<br>

# 공백을 피해주세요.

이 부분은 제가 다른 언어를 코딩하다보니까 생긴 습관이기도 한데요. 저는 코딩하면서 =사이에 습관적으로 공백을 넣더라구요. (c언어나 파이썬 등...) 하지만, HTML에서는 공백의 사용을 최대한 자제하라고 추천합니다.

```html
<link rel="stylesheet" href="style.css">
```
<br>

# 한 줄에 너무 길게 코딩하지 마세요.

이건 어느 언어를 사용할 때나 마찬가지 같아요. HTML 사용시에도 한 줄의 코드가 너무 길면 가독성이 떨어지니 다음 줄로 넘겨서 코딩해주세요.
<br>
<br>

# 과도한 줄바꿈이나 들여쓰기를 피해주세요.

아마 가독성을 위해서 줄바꿈이나 들여쓰기를 많이 사용하시는 분도 있으실텐데요. HTML 코딩에서는 간결함을 위해서 꼭 필요할 때만 줄바꿈과 들여쓰기를 사용해주세요.

아래 정도로만 사용해주세요!

```html
<<body>

<h1>HTML style guide</h1>

<h2>HTML style guide 01</h2>
<p>과도한 줄바꿈이나 들여쓰기를 피해주세요.</p>

</body>
```

아래처럼 과도한 줄바꿈 + 들여쓰기는 NO!
```html
<<body>

    <h1>HTML style guide</h1>

    <h2>HTML style guide 01</h2>

    <p>
        과도한 줄바꿈이나 들여쓰기를 피해주세요.
    </p>

</body>
```
<br>

# title을 빠뜨리지 마세요.

title은 필수적인 HTML 요소에요. 꼭 title을 작성해주세요. 물론, VS code에서 html code 작성 시 ! + enter키를 누르면 기본적으로 title 요소가 포함되어 나와요!

```html
<title>Gyubin's blog</title>
```
<br>

# \<html>과 를 \<body>를 빠뜨리지 마세요.

\<html>과 \<body>를 생략해도 코드가 동작은 해요. 하지만 몇몇 브라우저에서 또는 DOM, XML 소프트웨서는 동작하지 않을 수도 있어요!
<br>
<br>

# HTML comment는 이렇게 작성해주세요.

짧은 HTML 코멘트는 아래처럼 작성해주세요.

```html
<!-- This is a comment -->
```

두 줄 이상의 긴 HTML 코멘트는 아래처럼 작성해주세요.

```html
<!--
    This is a comment.
    This is a comment.
-->
```
<br>

# HTML에서 활용되는 파일 이름은 소문자를 사용하세요.

몇몇 브라우저에서는 소문자와 대문자를 체크해서 파일 이름에 접근하기도 해요. 그래서 모든 파일이름은 소문자를 사용해서, 혹여나 생길 문제를 방지하세요!
<br>
<br>

# Default file name을 체크해주세요.

URL의 끝에, 별도의 이름이 없다면 (e.g. https://gbsim.github.io) 기본적으로 "index.html", "index.html", "default.html" 등의 파일에 접근하게 되는데요.

서버 설정에 따라서 "index.html"에만 접근하도록 되어있을 수도 있으니, 꼭 설정을 확인하고 기본 html 파일의 이름을 적절하게 유지해주세요.

