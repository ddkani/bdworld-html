# 💡 사진 갤러리 만들기

반응형 사진 갤러리 페이지를 만들어봅시다. 그리드 레이아웃과 이미지 호버 효과를 활용해야 합니다.

## 요구사항

### HTML 구조
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>여행 사진 갤러리</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- 여기에 코드 작성 -->
</body>
</html>
```

### 필요한 요소들

1. **헤더 영역**
   - 갤러리 제목: `<h1>` "여행의 순간들"
   - 설명: `<p>` "세계 각지에서 담은 아름다운 풍경"

2. **필터 메뉴**
   - 카테고리 버튼들: 전체, 자연, 도시, 인물, 음식
   - `<nav>`와 버튼들로 구성

3. **갤러리 그리드**
   - 최소 8개의 사진
   - 각 사진은 `<figure>` 태그로 감싸기
   - 이미지: `<img>` 태그
     - Lorem Picsum 서비스 활용: `https://picsum.photos/너비/높이?random=번호`
     - 예: `https://picsum.photos/400/300?random=1`
     - 또는 실제 여행 사진 파일 사용
   - 캡션: `<figcaption>` 태그
   - 오버레이: `<div class="overlay">`

4. **사진 정보** (각 사진마다)
   - 제목
   - 촬영 장소
   - 촬영 날짜

### CSS 스타일링
- 그리드 레이아웃: 반응형 (모바일 1열, 태블릿 2열, 데스크톱 3-4열)
- 이미지 호버 효과:
  - 오버레이 표시
  - 확대 효과
  - 정보 표시
- 필터 버튼 활성화 스타일

### 힌트
- `display: grid`와 `grid-template-columns` 활용
- `overflow: hidden`으로 확대 효과 제한
- `transition`으로 부드러운 효과
- `:hover` 시 `transform: scale()` 사용
- `position: absolute`로 오버레이 구현
- **이미지 관련:**
  - Lorem Picsum은 랜덤한 고품질 사진을 제공하는 무료 서비스
  - `?random=` 파라미터로 각각 다른 이미지 로드
  - `width: 100%`와 `height: 100%`로 figure 크기에 맞추기
  - `object-fit: cover`로 비율 유지하며 채우기

### 참고 자료
- [이미지 넣기](https://www.yalco.kr/@html-css/1-5)
- [박스 모델](https://www.yalco.kr/@html-css/2-6)
- [위치 지정](https://www.yalco.kr/@html-css/2-9)
- [요소 숨기기](https://www.yalco.kr/@html-css/2-10)