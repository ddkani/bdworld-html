# 💡 이력서 페이지 만들기

전문적인 온라인 이력서를 만들어봅시다. 깔끔하고 읽기 쉬운 레이아웃으로 구성해야 합니다.

## 요구사항

### HTML 구조
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>홍길동 - 웹 개발자 이력서</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- 여기에 코드 작성 -->
</body>
</html>
```

### 필요한 요소들

1. **헤더 섹션**
   - 이름: `<h1>` "홍길동"
   - 직함: `<p>` "웹 개발자"
   - 연락처 정보: 이메일, 전화번호, GitHub 링크
   - 리스트(`<ul>`)로 구성

2. **자기소개 섹션**
   - 섹션 제목: `<h2>` "자기소개"
   - 소개 문단: 2-3개의 `<p>` 태그

3. **기술 스택 섹션**
   - 섹션 제목: `<h2>` "기술 스택"
   - 카테고리별로 구분:
     - Frontend: HTML, CSS, JavaScript, React
     - Backend: Node.js, Express, Python
     - Database: MySQL, MongoDB
   - 중첩 리스트 사용

4. **경력 사항 섹션**
   - 섹션 제목: `<h2>` "경력 사항"
   - 각 경력: `<article>` 태그
   - 회사명: `<h3>`
   - 기간: `<time>` 태그
   - 직책과 업무 내용: `<p>`와 `<ul>`

5. **학력 섹션**
   - 섹션 제목: `<h2>` "학력"
   - 학교명, 전공, 졸업년도

6. **프로젝트 섹션**
   - 섹션 제목: `<h2>` "프로젝트"
   - 프로젝트별 설명과 사용 기술

### CSS 스타일링
- 전체 최대 너비: 800px, 중앙 정렬
- 섹션별 구분선 또는 여백
- 인쇄 시에도 깔끔하게 보이도록 스타일링
- 링크 색상과 호버 효과

### 힌트
- 시맨틱 태그 활용 (`<header>`, `<section>`, `<article>`)
- 날짜는 `datetime` 속성과 함께 사용
- `::before` 선택자로 리스트 스타일 커스터마이징 가능
- `@media print`로 인쇄용 스타일 추가 가능

### 참고 자료
- [목록으로 나열하기](https://www.yalco.kr/@html-css/1-4)
- [용도와 중요도별 태그](https://www.yalco.kr/@html-css/1-2)
- [글자와 문단 스타일](https://www.yalco.kr/@html-css/2-2)