# 💡 카페 메뉴판 만들기

아늑한 카페의 메뉴판을 웹페이지로 만들어봅시다. 음료와 디저트 메뉴를 테이블로 정리해야 합니다.

## 요구사항

### HTML 구조
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cozy Cafe - 메뉴</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- 여기에 코드 작성 -->
</body>
</html>
```

### 필요한 요소들

1. **헤더 영역**
   - 카페 이름: `<h1>` "Cozy Cafe"
   - 슬로건: `<p>` "당신의 일상에 향기를 더합니다"

2. **메뉴 섹션**
   - 음료 메뉴
     - 섹션 제목: `<h2>` "☕ Beverages"
     - 테이블로 메뉴 구성
     - 컬럼: 메뉴명, 설명, 가격(Hot/Ice)
   
   - 디저트 메뉴
     - 섹션 제목: `<h2>` "🍰 Desserts"
     - 테이블로 메뉴 구성
     - 컬럼: 메뉴명, 설명, 가격

3. **푸터 영역**
   - 영업시간 정보
   - 연락처

### 테이블 구조
- `<thead>`와 `<tbody>` 구분
- 가격은 숫자와 원 단위 표시
- 음료는 Hot/Ice 가격 구분

### CSS 스타일링
- 테이블 스타일: `border-collapse: collapse`
- 헤더 배경: 갈색 계열 (#8B4513)
- 테이블 줄무늬 효과 (짝수 행)
- 호버 효과로 행 강조

### 힌트
- 테이블의 `<caption>` 태그를 활용할 수 있습니다
- `nth-child(even)` 선택자로 줄무늬 효과
- 가격 정렬은 `text-align: right`
- 테이블 전체 너비는 100%로 설정

### 참고 자료
- [표로 만들기](https://www.yalco.kr/@html-css/1-6)
- [색상 표현](https://www.yalco.kr/@html-css/2-4)
- [박스 모델](https://www.yalco.kr/@html-css/2-6)