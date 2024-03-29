# HTML

> 웹 브라우저에서 하이퍼텍스트 기능을 구현하는 웹페이지 작성 언어



## 태그

> - 기본적으로 <태그명> 내용</태그명> 구조를 갖는다.
>
> - 태그는 대소문자 구별 없이 사용



- 전체 기본 구조

``` html
<html>
    <head> 
        <meta charset="UTF-8">
        <title>탭제목</title>
        헤드 내용
    </head>
    <body>
        바디내용
    </body>
</html>
```

>HTML 은 기본적으로 2부분으로 나누어짐 HEAD 부분과 BODY 부분



- 태그의 구조 

  <태그 속성명="속성값"> 출력내용</태그>



태그 종류

- `<html>` :기본적으로 html 을 시작하고 끝낼때 사용하는 태그

- `<head>` : 타이틀, 메타태그, 스타일등을 작성하며 실제로는 표시되지 않는 부분

- `<body>` :기본 본문 내용(표시되는 부분)

- `<meta charset="UTF-8">` : 문자 코드 셋을 지정 UTF-8 로 지정하였다.

- `<title>` : 탭에 사용되는 텍스트 

- `<a href="주소" target="속성"> 이동 </a>` : 이동 클릭시 해당 주소로 이동
  - href속성(파일경로,이동할 사이트, 페이지 내의 특정 위치`#jQuery` 등)
  - target 속성(창을 여는 방식)
    - _self : 링크 클릭창에서 열기
    - _blank : 새창으로 열기
- `<link rel="stylesheet" type="text/css" href="css파일" />`:  보통 css 스타일 파일 사용
- `<h숫자>` : 제목 크기별 1~6 작을수록 큰 글자
- `<p>` : 문단을 나누는 태그(여러번 사용 시 간격이 벌어지지 않음.)
- `<!--주석내용-->` : 주석
- `<b>` : 강조
- `<i>` : 이탤릭체
- `<sub>` : 아래첨자/위첨자
- `<pre>` : 내용 그대로 인식 HTML 형태 그대로 유지
- `<span>` :  줄바꿈 없이 영역 묶기
- `<div> ` : 줄바꿈 있이 영역 묶기
- `<ul>` , `<ol>`, `<li>` : 기본 목록(순서없음. 순서있음) `<li>` 는 `ul,ol` 안에서 하나의 항목씩 표시

``` html
<ul>
    <li>목록1</li>
    <li>목록2</li>
</ul>
<ol>
    <li>목록1</li>
    <li>목록2</li>
</ol>
```

- `<dl>`, `<dt>`, `<dd>` : 정의 목록

``` html
<dl>
    <dt>항목</dt>
    <dd>설명</dd>
</dl>
```

- `<table>` : 태이블 생성 태그
- `<tr>`, `<td rowspan="숫자">` : 한행마다 생성, 한 목록마다 생성
  - rowspan : 숫자만큼 세로 병합, colspan: 숫자만큼 가로 병합
  - border : 테이블 경계선 굵기
  - width : 너비지정 (픽셀이나, % 사용가능
  - height : 너비지정 (픽셀이나, % 사용가능)
  - cellpadding : 셀과 경계선 사이 여백
  - cellspacing : 셀과 셀 사이 여백
  - align : 가로정렬
  - valgin : 세로정렬

``` html
<table>
    <tr><td></td><td></td></tr>
    <tr><td></td><td></td></tr>
</table>
```

- `<img src="경로" alt="이미지없을때 대체출력" usemap="#이름">` : 이미지 삽입
  - usemap (이미지 내부에서 영역을 정하기)
- `<iFrame>` : 문서속에 문서
- `<audio src="경로">` : 오디오 파일
  - preload : 재생하기 전에 오디오 파일 모두 로드
  - loop : 반복재생
- `<video src="경로">` : 비디오 파일 재생
  - poster : 비지오 준비중 이미지
- `<track>` : 자막(.vtt)
- `<form>` : 입력 양식 태그
- `<label>` : 폼 요소에 캡션 붙이기
- `<input>` : 데이터 입력 받는 태그
  - type : radio , checkbox
  - size
- `<slect>` : 드롭다운 목록 표시







줄바꿈 없이 쓸 수 있는 태그

- `<br>` : 줄바꿈
- `<img>` : 이미지 삽입
- `<hr>` : 수평선 삽입
- `&nbsp;` : 공백문자
- `&copy;` &copy;



시멘틱

`<nav>`

`<aside>`

`<section>`

`<article>`

`<footer>`



HTML5 시멘틱 구조의 특징
 - 이전 웹 브라우저와 보이는 모습은 동일 
 - 실제로 웹 브라우저에서 문서를 처리할 때 차이
 - 소스만으로도 문서 내용 쉽게 파악 (태그만 보고도 제목, 메뉴, 내용 등을 쉽게 구분)
 - 편리한 검색 : 검색 시 필요한 내용을 정확하게 찾을 수 있음

 HTML5 시멘틱 구조의 장점
 - 소스만으로 문서 내용 쉽게 파악
 - 편리한 검색
 - 뛰어난 웹 접근성 : 제목과 내용 등 구별 -> 사용자에게 정확한 내용 전달 가능
 - 다양한 장치에 동일된 결과 제공 (태그 역할이 정해져 있기 때문에 어떤 장치에서든 통일하게 문서 해독 가능)



