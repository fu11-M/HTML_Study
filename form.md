##<form> : 
사용자에게 정보를 입력 받는 요소이며 태그를 통해 사용자가 제출한 데이터를 서버에 전송할 때 사용된다. 
사용자가 제출한 데이터를 서버에 전송할 때 사용되는 <form>태그의 속성은 action(전송 위치), method(전송 방식)을 사용하며 대표적으로 회원 가입 및, 로그인 페이지 양식이 대표적이다. 

#method의 전송 방식에는 GET과 POST방식이 존재하며 GET과 POST는 HTTP 프로토콜에서 사용된다.

#GET : 
사용자의 데이터를 서버로 전송하는 용도와 서버에서 사용자에게 페이지를 요청하는데 사용되며 주로 데이터를 서버에서 가져와 사용자에게 제공되는 용도로 사용된다. 

사용자의 데이터를 URL의 쿼리 문자열로 표현하며 ***쿼리 문자열은 URL 끝에 있는 ?표시로 시작하고*** <key = value> 형식으로 데이터가 전달된다. 즉, GET은 URL에 데이터를 첨부하여 전송된다.

하지만 URL의 길이에는 제한이 있어 데이터의 크기가 제한 적이기 때문에 전송되는 데이터의 양이 제한적이고 데이터가 URL에 첨부되어 전송 하는 정보가 URL에 그대로 노출 되기 때문에 보안에 취약하다.

##Get_Ex

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>form</title>
</head>
<body>
    <form method="get">
        <input type="text" name = "search">
        <input type="submit">
    </form>
</body>
</html>
```
![alt text](init.png)

init을 입력하고 제출을 클릭하게 되면 

![alt text](init_Result.png)


get method로 보낸 데이터가 URL에 표시된다.


#POST : 
주로 데이터를 서버로 제출할 때 사용되며 GET과 달리 HTTP 요청의 본문(body)에 데이터를 포함 시켜 전송하기 때문에
URL의 길이와 상관 없이 데이터를 전달할 수 있어 데이터의 크기에 제한이 없고 요청한 데이터를 URL에 표시 하지 않아
GET 방식 보다 안전하다.

##Post_Ex)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>form</title>
</head>
<body>
    <form method="post">
        <input type="text" name = "search">
        <input type="submit">
    </form>
</body>
</html>
```

![alt text](init_post.png)

init을 입력하고 제출을 클릭하게 되면

![alt text](init_post_result.png)

POST method로 보낸 데이터가 URL에 표시 되지 않고 HTTP 요청의 본문 내부에 데이터를 포함 시킨다.

