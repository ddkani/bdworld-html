# 💡 할 일 목록 만들기

간단하면서도 실용적인 할 일 목록(Todo List) 페이지를 만들어봅시다. 체크박스와 우선순위 표시 기능을 포함해야 합니다.

## 요구사항

### HTML 구조
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>나의 할 일 목록</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- 여기에 코드 작성 -->
</body>
</html>
```

### 필요한 요소들

1. **헤더 영역**
   - 제목: `<h1>` "오늘의 할 일"
   - 날짜 표시: `<time>` 태그 사용

2. **할 일 추가 섹션**
   - 입력 필드: `<input type="text">`
   - 우선순위 선택: `<select>` (높음, 보통, 낮음)
   - 추가 버튼: `<button>`

3. **할 일 목록**
   - 카테고리별 섹션:
     - 오늘 할 일
     - 이번 주 할 일
     - 완료된 일
   - 각 할 일 항목:
     - 체크박스: `<input type="checkbox">`
     - 할 일 내용: `<label>`
     - 우선순위 표시: `<span class="priority">`
     - 삭제 버튼

4. **통계 섹션**
   - 전체 할 일 개수
   - 완료된 일 개수
   - 완료율 표시
   - 진행률 바 (Progress Bar)

### 예시 할 일 항목
- 프로젝트 기획서 작성 (높음)
- 팀 미팅 참석 (보통)
- 이메일 확인 및 답장 (낮음)
- 코드 리뷰 (높음)
- 점심 약속 (보통)
- 운동하기 (낮음)

### CSS 스타일링
- 우선순위별 색상 구분 (높음: 빨강, 보통: 주황, 낮음: 초록)
- 완료된 항목 스타일 (취소선, 흐린 색상)
- 체크박스 커스터마이징
- 호버 효과
- 반응형 디자인
- **그라데이션 효과:**
  - 헤더 배경: `background: linear-gradient(135deg, #667eea 0%, #764ba2 100%)`
  - 버튼 배경: `background-color` 대신 `background: linear-gradient()` 사용
  - Progress Bar: 그라데이션으로 시각적 효과 증대

### 힌트
- `:checked` 선택자로 체크된 항목 스타일링
- `text-decoration: line-through`로 취소선
- `opacity`로 완료된 항목 흐리게
- 우선순위별 `border-left` 색상 구분
- **Progress Bar 구현 방법:**
  - 바깥 컨테이너: `<div class="progress-bar">`
  - 내부 진행률: `<div class="progress" style="width: 30%">`
  - `transition` 속성으로 부드러운 애니메이션
- **그라데이션 문법:**
  - `linear-gradient(방향, 색상1 위치1, 색상2 위치2)`
  - 방향: `to right`, `to bottom`, `135deg` 등
  - 예: `background: linear-gradient(90deg, #667eea 0%, #764ba2 100%)`

### 참고 자료
- [사용자 입력 받기](https://www.yalco.kr/@html-css/1-9)
- [목록으로 나열하기](https://www.yalco.kr/@html-css/1-4)
- [글자와 문단 스타일](https://www.yalco.kr/@html-css/2-2)
- [배경 스타일링](https://www.yalco.kr/@html-css/2-8)