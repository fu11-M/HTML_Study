- 공간 분할 태그
<div> : 구획을 나누거나 그룹 화 할 때 사용된다. 그룹화 하게 되면 그룹화 된 영역을 스타일링(CSS), 스크립팅(JS), 레이아웃을 구성하고 관리하는데 용이하다.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <div>div block1</div>
    <div>div block2</div>
    <div>div block3</div>
    <div>div block4</div>
    <div>div block5</div>
    <div>div block6</div>
</body>
</html> 
```

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ea204791-94b0-4594-95e9-37705edf8245/781645ba-08a1-474e-a12b-4c3fe8b69c05/Untitled.png)

<span> : 텍스트나 이미 등의 인라인 요소를 그룹화 할 때 사용된다. 인라인 요소를 그룹화 하여 <div>와 마찬가지로 스타일링(CSS), 스크립팅(JS), 레이아웃을 구성하고 관리하는데 용이하다.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <span>/span inline/</span>
    <span>/span inline/</span>
    <span>/span inline/</span>
    <span>/span inline/</span>
    <span>/span inline/</span>
    <span>/span inline/</span>
</body>
</html> 
```

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ea204791-94b0-4594-95e9-37705edf8245/28a50aa7-267d-4670-8e03-0c6bc32d5075/Untitled.png)

<div>, <span> 둘의 차이점 :

줌 바꿈 : div는 줄 바꿈이 되지만 span 태그는 줄 바꿈이 되지 않고 옆으로 붙는다.

영역을 지정하는 방식 : div태그는 텍스트를 표현할 때 사각형 박스로 구역을 정하지만 span은 문장 단위로 지정한다.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>입력폼 실습</title>
</head>
<body>
    <form action="https://search.naver.com/search.naver">
        <fieldset>
            <legend>네이버 검색</legend>
            <input type="text" name = "query" required="true">
            <button type="submit">검색</button>
        </fieldset>
    </form>

    <form action="" method="post">
        <fieldset>
            <legend>기본 정보</legend>
            <ul>
                <li>이름: <input name="name" type="text" placeholder="실명을 입력해주세요."> </li>
                <li>나이: <input name="age" type="number" value="0" min="0" max="200"> </li>
                <li>비밀번호: <input name="pw" type="password"></li>
            </ul>
        </fieldset>

        <fieldset>
            <legend>부가정보</legend>
            <li>
                거주지역
                <select name="loc" id="">
                    <option value="서울">서울</option>
                    <option value="경기">경기</option>
                    <option value="경상도">경상도</option>
                    <option value="제주도">제주도</option>
                </select>
            </li>
            <li>
                기술:
                <input type="checkbox" name="" id="cb1"> 
                <label for = "cb1">HTML</label>
                <input type="checkbox" name="" id="cb2"> 
                <label for = "cb2">CSS</label>
                <input type="checkbox" name="" id="cb3"> 
                <label for = "cb3">JS</label>
            </li>
            <li>
                과정:
                <input type="radio" name="과" id="rd1">
                <label for="">통학</label>
                <input type="radio" name="과" id="rd1">
                <label for="">기숙사</label>
                <input type="radio" name="과" id="rd1">
                <label for="">자퇴</label>
            </li>
        </fieldset>
        <button type="submit">제출</button>
    </form>
    
</body>
</html>
```

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ea204791-94b0-4594-95e9-37705edf8245/876db6b5-52cb-4070-a617-6d8c827a4aad/Untitled.png)

![Untitled](https://prod-files-secure.s3.us-west-2.amazonaws.com/ea204791-94b0-4594-95e9-37705edf8245/b9d8e40c-3e93-4d9d-bb11-29a50b0d5562/Untitled.png)