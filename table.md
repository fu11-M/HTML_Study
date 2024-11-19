## table 태그
### table :  표 삽입 / border속성을 사용하여 표의 테두리 두께를 지정할 수 있다.
### tr : 표의 행 삽입
### th : 표의 제목 셀 생성 / colspan 속성 → 셀의 너비, rowspan 속성 → 셀의 높이를 설정할 수 있다.
### td : 표의 일반 셀 생성 / colspan 속성 → 셀의 너비, rowspan 속성 → 셀의 높이를 설정할 수 있다.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    table {
        border: 3px solid black;
        border-collapse: collapse;
    }

    td{
        border: 1px solid black;
        width: 100px;
        height: 100px;
        text-align: center;
        font-size: 20pt;
    }
</style>
<body>
    <table style="width: 50%;">
       
        <tr>
                <td colspan="5"></td>
        </tr>
        <tr>
                <td rowspan="4"></td>
                <td colspan="4"></td>
        </tr>
        <tr>
                <td></td>
                <td rowspan="2"></td>
                <td></td>
                <td rowspan="3"></td>
        </tr>
        <tr>
                <td></td>
                <td></td>
        </tr>
        <tr>
                <td colspan="2"></td>
                <td></td>
        </tr>
    </table>
</body>
</html>---
```

<!--  -->
![alt text](./img/table.img/table.png)
<!--  -->
___

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    table {
        border: 3px solid black;
        border-collapse: collapse;
    }

    td{
        border: 1px solid black;
        width: 100px;
        height: 100px;
        text-align: center;
        font-size: 20pt;
    }
</style>
<body>
    <table style="width: 50%;">
        <tr>
            <td></td>
            <td>월</td>
            <td>화</td>
            <td>수</td>
            <td>목</td>
            <td>금</td>
        </tr>

        <tr>
            <td>1교시</td>
            <td rowspan="3">Java</td>
            <td rowspan="2">HTML</td>
            <td colspan="3", rowspan="3">Spring</td>
        </tr>

        <tr>
            <td>2교시</td>
        </tr>

        <tr>
            <td>3교시</td>
            <td rowspan="3">CSS</td>
        </tr>

        <tr>
            <td>4교시</td>
            <td rowspan="2">JS</td>
            <td rowspan="4">JSP</td>
            <td colspan="2">GIT</td>
        </tr>

        <tr>
            <td>5교시</td>
            <td rowspan="3">CS</td>
            <td rowspan="3">React</td>
        </tr>

        <tr>
            <td>6교시</td>
            <td rowspan="2">DB</td>
            <td rowspan="2">JS</td>
        </tr>

        <tr>
            <td>7교시</td>
        </tr>
</table>
</body>
</html>
```

<!--  -->
![alt text](./img/table.img/table2.png)
<!--  -->
___

