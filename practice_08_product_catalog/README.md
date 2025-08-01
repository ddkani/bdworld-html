# 💡 제품 카탈로그 만들기

온라인 쇼핑몰의 제품 카탈로그 페이지를 만들어봅시다. 그리드 레이아웃으로 제품들을 보기 좋게 배치해야 합니다.

## 요구사항

### HTML 구조
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tech Shop - 제품 카탈로그</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- 여기에 코드 작성 -->
</body>
</html>
```

### 필요한 요소들

1. **헤더 영역**
   - 쇼핑몰 이름: `<h1>` "Tech Shop"
   - 네비게이션: `<nav>`와 `<ul>` 사용
     - 메뉴: 노트북, 스마트폰, 액세서리, 고객지원

2. **메인 콘텐츠**
   - 페이지 제목: `<h2>` "인기 상품"
   - 제품 그리드: `<div class="product-grid">`
   
3. **각 제품 카드** (최소 6개)
   - 제품 이미지: `<img>` 태그 사용
     - placeholder 서비스 활용 가능: `https://placehold.co/300x200/색상코드/텍스트색상?text=제품명`
     - 예: `https://placehold.co/300x200/e3e3e3/666?text=MacBook+Pro`
     - 또는 실제 제품 이미지 파일 사용
   - 제품명: `<h3>`
   - 가격: `<p class="price">`
   - 간단한 설명: `<p>`
   - 장바구니 버튼: `<button>`

4. **제품 예시**
   - 맥북 프로 14인치
   - 아이폰 15 Pro
   - 갤럭시 S24 Ultra
   - 에어팟 프로
   - 애플 워치 시리즈 9
   - 아이패드 프로

### CSS 스타일링
- 제품 그리드: 3열 레이아웃 (화면 크기에 따라 반응형)
- 제품 카드: 그림자 효과, 호버 시 확대
- 가격: 강조 색상과 큰 글씨
- 버튼: 호버 효과

### 힌트
- `display: grid` 또는 `display: flex` 활용
- `grid-template-columns: repeat(3, 1fr)`로 3열 만들기
- `transform: scale(1.05)`로 호버 확대 효과
- `box-shadow` 속성으로 카드 그림자 효과
- **이미지 스타일링:**
  - `width: 100%`로 카드 너비에 맞추기
  - `height: 200px`와 `object-fit: cover`로 일정한 높이 유지
  - `border-radius`로 모서리 둥글게

### 참고 자료
- [인라인과 블록 요소](https://www.yalco.kr/@html-css/2-5)
- [박스 모델](https://www.yalco.kr/@html-css/2-6)
- [위치 지정](https://www.yalco.kr/@html-css/2-9)