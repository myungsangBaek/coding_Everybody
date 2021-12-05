# coding_Everybody

HTML, CSS, JS 기본기를 다시 다지기위해 생활코딩을 정주행하며 만들어본 예제들입니다.

### 태그

옷에 달린 tag처럼 text를 어떻게 나타낼지 설명한다.

`<strong>` : bold체
`<h1>` ~ `<h6>` : 제목

### 줄바꿈

`<br>` : 한 줄이 떨어진다. 여러 번 사용 가능하다.
`<p>` : 문단이 나눠진다. 정해진만큼의 여백만 벌어지기에 시각적 자유도가 떨어진다.

웹은 접근성이 중요하며, 신체적 결함이 있는분들도 정보들로부터 소외되지 않도록 노력해야한다.

### 속성

`<img src="">`태그 내의 src 부분을 속성(Attribute)이라고 한다. 이 속성은 위치는 상관없고 태그만으로 정보가 부족할 때 사용한다.

### 목차

`<li>` : list의 약자로 목차용 태그로 사용한다.
`<ul>` : Unordered List의 약자로 <li>태그의 부모로 리스트의 구분을 줄 수 있다.
`<ol>` : Ordered List의 약자로 자동으로 숫자가 넘버링 된다.

### 문서의 구조

`<title>` : 이 태그를 사용하면 본문의 제목을 변경할 수 있다.

컴퓨터는 0101 이진법만 처리하기 때문에 한글을 바로 사용하면 깨짐 현상이 일어나기에 UTF-8로 열릴 수 있도록 <meta charset="utf-8">를 작성해주어야 한다.
char은 문자 set은 규칙을 뜻한다.

이 코드들은 <head>태그로 묶이며 본문을 설명해준다.

본문은 <body> 태그로 묶인다.

이 두가지를 <html> 테그로 묶는다. 이 위에 관용적으로 <!doctype html>로 표시한다.

### 링크

`<a>` : anchor의 약자로 링크 태그이다. 이 태그로 인해 다른 사이트들이 고립되지않고 공유될 수 있다. 사이트끼리 연결하는 본드나 실의 역할

```HTML
<a href="", target="_blank" title="html"  > : 링크 넣는 장소, 새 탭 열기, 마우스 올리면 설명 나오기 (툴팁)
```
