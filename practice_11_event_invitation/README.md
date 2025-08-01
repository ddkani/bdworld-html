# 💡 이벤트 초대장 만들기

세련된 이벤트 초대장 페이지를 만들어봅시다. 배경 이미지와 텍스트 스타일링을 활용해 매력적인 디자인을 구현해야 합니다.

## 요구사항

### HTML 구조
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tech Conference 2024 - 초대장</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- 여기에 코드 작성 -->
</body>
</html>
```

### 필요한 요소들

1. **메인 컨테이너**
   - 전체 화면 높이 사용 (`min-height: 100vh`)
   - 배경 이미지 또는 그라데이션

2. **이벤트 정보**
   - 이벤트 명: `<h1>` "Tech Conference 2024"
   - 부제: `<p class="subtitle">` "미래를 만드는 기술의 향연"
   - 날짜/시간: `<time>` "2024년 5월 15일 오후 2시"
   - 장소: `<address>` "서울 코엑스 그랜드볼룸"

3. **이벤트 설명**
   - 이벤트 소개 문단
   - 주요 연사 정보 (리스트)
   - 프로그램 일정

4. **참가 신청 섹션**
   - 참가 신청 버튼 (큰 CTA 버튼)
   - 문의사항 연락처

5. **특별 요소**
   - 인용문: `<blockquote>` 사용
   - 강조 텍스트: `<strong>`, `<em>` 활용

### CSS 스타일링
- 배경: 그라데이션 또는 이미지 오버레이
- 텍스트 그림자로 가독성 향상
- 중앙 정렬된 콘텐츠
- 애니메이션 효과 (fade-in 등)
- 반응형 디자인
- **그라데이션 효과 활용:**
  - 메인 배경: 다중 레이어 그라데이션
  - 버튼: 그라데이션으로 입체감 표현
  - 오버레이: 투명도 그라데이션으로 텍스트 가독성 향상

### 힌트
- `background-image`와 `linear-gradient` 조합
- `text-shadow`로 텍스트 강조
- `@keyframes`로 애니메이션 정의
- `::before`, `::after` 가상 요소 활용
- **그라데이션 예제:**
  ```css
  /* 다중 그라데이션 배경 */
  .invitation-container {
    background: 
      linear-gradient(135deg, rgba(25, 25, 112, 0.9), rgba(138, 43, 226, 0.9)),
      url('background.jpg') center/cover;
  }
  
  /* 버튼 그라데이션 */
  .cta-button {
    background: linear-gradient(45deg, #ff6b6b, #ff8787);
  }
  
  /* 섹션 배경 그라데이션 */
  section {
    background: rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(5px);
  }
  
  /* 오버레이 그라데이션 */
  .overlay {
    background: linear-gradient(to bottom, 
      rgba(0,0,0,0) 0%, 
      rgba(0,0,0,0.7) 100%);
  }
  ```

### 참고 자료
- [인용된 콘텐츠](https://www.yalco.kr/@html-css/1-3)
- [배경 스타일링](https://www.yalco.kr/@html-css/2-8)
- [위치 지정](https://www.yalco.kr/@html-css/2-9)