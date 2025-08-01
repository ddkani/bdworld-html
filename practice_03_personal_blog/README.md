# 💡 개인 블로그 페이지 만들기

개인 블로그의 메인 페이지를 만들어봅시다. 제목, 자기소개, 최근 포스트 목록을 포함해야 합니다.

## 요구사항

### HTML 구조
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>나의 개발 블로그</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- 여기에 코드 작성 -->
</body>
</html>
```

### 필요한 요소들

1. **헤더 영역**
   - 블로그 제목: `<h1>` 태그 사용
   - 부제목: `<p>` 태그로 "프로그래밍과 일상을 기록합니다"

2. **자기소개 섹션**
   - 섹션 제목: `<h2>` "About Me"
   - 프로필 이미지: placeholder 이미지 사용 가능 (alt 텍스트 포함)
     - 예: `https://placehold.co/200x200/667eea/ffffff?text=Profile`
     - 또는 `https://picsum.photos/200/200` (랜덤 이미지)
     - 또는 본인의 실제 이미지 파일 사용
   - 자기소개 문단: 2-3개의 `<p>` 태그

3. **최근 포스트 섹션**
   - 섹션 제목: `<h2>` "최근 포스트"
   - 포스트 목록: `<article>` 태그로 각 포스트 감싸기
   - 각 포스트에는:
     - 제목: `<h3>` 태그
     - 날짜: `<time>` 태그
     - 요약: `<p>` 태그
     - "더 읽기" 링크: `<a>` 태그

### CSS 스타일링

- 전체 페이지 최대 너비: 800px, 중앙 정렬
- 헤더 배경색: `#333`, 글자색: 흰색
- 포스트 간격: 20px
- 링크 호버 효과 추가

### 힌트

- 시맨틱 태그(`<header>`, `<main>`, `<section>`, `<article>`)를 활용하세요
- 이미지는 `width: 200px`, `border-radius: 50%`로 원형 처리
- 날짜는 `datetime` 속성을 포함한 `<time>` 태그 사용
- CSS의 `:hover` 선택자로 링크 효과 구현

### 참고 자료
- [제목과 본문](https://www.yalco.kr/@html-css/1-1)
- [이미지 넣기](https://www.yalco.kr/@html-css/1-5)
- [다른 곳으로의 링크](https://www.yalco.kr/@html-css/1-7)
- [박스 모델](https://www.yalco.kr/@html-css/2-6)