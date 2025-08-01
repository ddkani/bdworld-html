> 💡 레이아웃 만들기
> 

전체 페이지 내에 컨테이너가 있고, 컨테이너 안에 “학기별 성적정보 조회" 및 테이블이 구성되어 있다.

```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>학생정보조회시스템</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <div class="container">
        <!-- 여기에 코드 작성 -->
    </div>
</html>
```

CSS 레이아웃을 이용하여 디자인을 완성한다.

- class=container div
    - 페이지 전체 (body) 의 배경색과 컨테이너의 배경색이 다르다.
        - 페이지 배경: `#f4f4f4`
        - 컨테이너: `#ffffff`
        - 컨테이너는 배경색 뿐 만 아니라 테두리도 가지고 있다.
    - 컨테이너의 크기와 위치 (가운데 정렬)을 하기 위한 방법은?
- 테이블
    - 테이블 역시 각 행과 열에 모두 테두리가 있다.
    - 테이블의 모든 글은 왼쪽 정렬한다.
    - 그림과 같이 테이블의 모든 행과 열이 붙어 있도록 하려면?
        - `border-collapse: collapse`
    - 테이블의 각 행과 열에 적절한 여백 주기
