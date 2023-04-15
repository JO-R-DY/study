# 시작하기
>1. 프로젝트 폴더, 파일(html,css,js) 생성
>2. css 초기화 (reset.css)
[reset-css CND](https://www.jsdelivr.com/package/npm/reset-css)
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/reset-css@5.0.1/reset.min.css">
```
💬 reset이 main.css보다 밑에 줄에 있으면 초기화된 style로 반영되기 때문에 main.css 보다 위에 작성해야함.
>3. script, css 연결
```html
<script defer src="./main.js"></script>
```
```html
<link rel="stylesheet" href="./main.css">
```

>4. 폰트연결
- 구글 ([Google Fonts](https://fonts.google.com/)에서 고른 폰트 파일을 가져옵니다.)

html
```html
<link rel="preconnect" href="https://fonts.gstatic.com" />
<link href="https://fonts.googleapis.com/css2?family=Nanum+Gothic:wght@400;700&display=swap" rel="stylesheet" />
```

css

```css
body {
    font-family: 'Nanum Gothic', sans-serif;
}
```
- 나눔스퀘어네오

css

```css
@font-face {
  font-family: 'NanumSquareNeo-Variable';
  src: url('https://cdn.jsdelivr.net/gh/projectnoonnu/noonfonts_11-01@1.0/NanumSquareNeo-Variable.woff2') format('woff2');
  font-style: normal;
}

body{
  font-family: "NanumSquareNeo-Variable";
  font-weight: 300;
}
```
- 프리텐다드

html

```html
<link rel="preload" as="style" crossorigin href="https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.6/dist/web/variable/pretendardvariable.css">
```
css

```css
@import url("https://cdn.jsdelivr.net/gh/orioncactus/pretendard@v1.3.6/dist/web/variable/pretendardvariable.css");

body{
  font-family: "Pretendard Variable", Pretendard, -apple-system, BlinkMacSystemFont, system-ui, Roboto, "Helvetica Neue", "Segoe UI", "Apple SD Gothic Neo", "Noto Sans KR", "Malgun Gothic", "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", sans-serif;
  font-weight: 300;
}
```
