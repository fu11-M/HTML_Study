### HTML은 HyperText Markup Language(하이퍼텍스트 마크업 언어)의 약자로, 웹 페이지를 만들기 위한 가장 기본적인 마크업 언어이다. 

HTML은 웹 페이지의 기본적인 구조를 형성하는데 사용되며 텍스트 기반으로 작성되어 태그(tag)를 사용하여 텍스트, 이미지, 링크 등 문서의 각 콘텐츠를 정의한다. 

CSS3를 사용한 웹 페이지의 스타일링과 javaScript를 사용한 웹의 동적인 기능을 추가할 수 있다. 

웹은 요청과 응답이라는 형태로 동작하고 클라이언트가 브라우저에서 특정 웹 서버의 주소를 입력(요청)하면 해당 브라우저의 웹 서버에서 

요청한 주소의 웹 페이지인 HTML 페이지를 제공(응답)한다.

## Client → Request → Server

## Server → Response → Client

### (웹에서 어떤 대상을 구분하는 방법을 총칭 하는 URI중 주소로 구분하는 것이 URL이다.)

즉, 클라이언트가 HTML페이지를 요청하면 서버가 해당 요청에 응답하여 요청한 HTML 페이지를 제공한다는 것이며 웹은 클라이언트와 
서버 사이의 통로인 것이다.

클라이언트 즉 요청하는 프로그램을 만들기 위해 필요한 웹 표준 기술은 HTML5표준, CSS3표준, javascript(ECMAScript)표준 3가지의 기술을 사용한다.

 - HTML는 웹 페이지를 구성하는 HTML 마크업 언어를 뜻하며 웹페이지의 서식이나 구조와 같은 기본틀을 표현할 때 사용하는 기술
 - CSS3는 HTML 페이지에 스타일을 지정하는 스타일 시트를 작성할 때 사용하는 기술
 - javascript는 HTML페이지 에서 사용자 반응 등을 처리하는 스크립트를 작성하는 기술

HTML은 크게 head태그와 body태그로 나뉘며 head 태그는 웹 페이지의 정보를 담고 있고 , body 태그는 웹 페이지의 실제 내용이 담겨 있는 것이라고 생각하면 된다.

head태그는 페이지의 다양한 정보를 담고 있으며 이 정보들은 브라우저에는 표시되지 않고, 웹 페이지의 정보를 정의하거나 외부 리소스와의 연결을 설정하는데 사용된다.

### !DOCTYPE html : 이 파일은 html로 구성되어 있음

### html lang="en" :  html언어는 영어

```html
<!DOCTYPE html> 
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title></title>
</head>

<body>
    
</body>
</html>
```

## head태그 내부에 포함되는 요소 

 - title : 
웹 페이지의 제목 정의 (브라우저 탭이나 페이지의 제목 표시줄에 표시됨)

 - meta : 
웹 페이지의 메타데이터를(데이터에 대한 추가 정보) 정의 (인코딩, 페이지 설명, 키워드)

 - link : 
외부 리소스(다양한 형태의 데이터)와의 연결을 설정하며 주로 CSS파일, favicon(아이콘 표시 이미지 파일)과 같은 것들을 불러올 때 사용된다.

 - style : 
CSS스타일로 HTML문서 전체를 정의  /  인라인 style(HTML 요소에 style 속성을 직접 지정하는 것)

### - script : 
외부 JavaScript 파일을 연결하거나, 인라인 JavaScript코드를 포함할 때 사용

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="keywords" content="HTML, CSS, JavaScript"> 
    <link rel="stylesheet" href="MyEx1.css">
    <link rel="icon" href="MyEx1.ico" type="image/icon">
    <title>MyEx1</title>
    <style>
        body{
            color: black;
            background-color: cadetblue;
        }
    </style>
</head>
<body>
    welcome to my Ex1
    <script src="MyEx1.js"></script>
    <script>
    console.log("my Ex1에 오신걸 환영합니다")
    </script>
</body>
</html>
```
<!--  -->
![alt text](./img/html.img/html.png)
<!--  -->

<!--  -->
![alt text](./img/html.img/console.png)
<!--  -->