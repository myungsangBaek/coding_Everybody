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

### 웹의 역사

1960년 인터넷의 탄생하였고, 1990년에 Web이 등장하였다.

###### 웹의 메소포타미아

info.cern.ch

### 서버와 클라이언트

Web Browser(client컴퓨터)에서 Web Server(server컴퓨터)로 요청(request)을 보내면 Web Server에서 index.html을 찾아서 응답(response)한다.

### 웹호스팅

Web server를 연결하기 위한 컴퓨터를 Host라고 한다. 웹서버를 제공해주는 회사를 웹호스팅 업체라고 한다.

GitHub에서도 무료로 호스팅이 가능하다.

Settings -> GitHub Pages -> Source(none -> 해당branch) -> Save

각 컴퓨터의 웹서버 주소
http://127.0.0.1/ <= **I**nternet **P**rotocol **Address**

http(Hyper Text Transfer Protocol)는 Web Browser과 Web Server과 통신할 때 사용하는 통신규약이다.

## CSS

### 기본 문법

1. <style> 태그를 사용하여 css 효과를 줄 수 있다.

```CSS
<style>
    a{
        color:red;
    }
</style>
```

2. style 속성을 사용하여 css 효과를 줄 수 있다.

### class

class 속성을 주면 특정 값에 css 효과를 줄 수 있다. class 선택자는 '.'이다.

여러 개의 클래스의 영향을 받는 경우 가까이 있는 명령이 더 큰 영향이 있기 때문에 class는 그다지 좋은 방법은 아니다.

### id

그래서 사용하는 것이 'id'이다. id 선택자는 '#'이다. 그러면 순서와 관계없이 속성을 적용시킬 수 있다.

##### 강한 순서

태그 선택자 < class 선택자 < id 선택자

그 이유는 id선택자의 값은 web에서 한 번만 등장할 수 있다. (중복되서는 안된다.) 유일무이하다.
좀 더 구체적인 것이 포괄적인 것보다 우선순위가 높다.

### box model

틀을 잡기 위해서는 box model이라는 개념이 중요하다.

<h1>태그는 줄바꿈이 자동으로 되나 <a> 태그는 줄바꿈이 되지않고 다른 콘텐츠들과 같은 라인에 위치한다.

이유는 링크는 자기 크기만큼 사용하고 <h1>태그는 화면 전체를 사용하는 태그이기 때문이다.

테두리를 넣어주면 부피감을 알 수 있다.

여기서 화면전체를 사용하는 태그를 'block level element'라고 한다.

자기 자신의 크기만큼 사용하는 태그를 'inline element'라고 한다.

display를 사용하여 서로 속성을 변경할 수 있다.

```CSS
display : block;
display : inline;
```

padding : 컨텐츠와 테두리의 간격
margin : 테두리 사이의 간격
width : 너비

![BOX MODEL](data:image/png;base64,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)

개발자 도구에 들어가면 content, padding, border, margin을 볼 수 있다.
