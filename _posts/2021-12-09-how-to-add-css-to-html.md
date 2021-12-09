---
layout: post
title: html에 css를 넣는 법 
categories: css
tags: [css, html]
---

### 1. 같은 html파일에 css 코드 적기

같은 HTML 파일에 CSS 코드를 입히는 방법으로는 'style'태그를 이용한다.(이 때, head 안에 있어야 한다.)

```html!
<head>
<style></style>
</head>
```

### 2. css와 html을 분리하는 방법

- CSS를 분리시켜 만들 때는 따로 CSS 파일을 만든다
- HTML 파일에서 'link' 태그를 이용하여 CSS 파일과 연결한다.
- styles.css와 이 HTML과의 관계를 말할 때, styles.css는 스타일시트라 한다.
- rel(relationship 관계)에 대해 명시해야 한다.

```html!
<head>
<link href="styles.css" rel="stylesheet" />
</head>
```



