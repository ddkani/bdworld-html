# 💡 뉴스레터 구독 페이지 만들기

매력적인 뉴스레터 구독 랜딩 페이지를 만들어봅시다. 사용자의 관심을 끌고 구독을 유도하는 디자인을 구현해야 합니다.

## 요구사항

### HTML 구조
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tech Weekly - 주간 기술 뉴스레터</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- 여기에 코드 작성 -->
</body>
</html>
```

### 필요한 요소들

1. **히어로 섹션**
   - 제목: `<h1>` "Tech Weekly"
   - 부제: `<p>` "매주 월요일, 최신 기술 트렌드를 당신의 메일함으로"
   - 배경 이미지 또는 그라데이션

2. **혜택 소개**
   - 섹션 제목: `<h2>` "구독자 혜택"
   - 혜택 리스트 (아이콘과 함께):
     - 주간 기술 뉴스 요약
     - 독점 인터뷰 및 분석
     - 개발 팁과 튜토리얼
     - 무료 전자책 다운로드

3. **구독 폼**
   - 이메일 입력: `<input type="email">` 
   - 관심 분야 선택 (체크박스):
     - AI/머신러닝
     - 웹 개발
     - 모바일
     - 클라우드
   - 구독 버튼
   - 개인정보 동의 체크박스

4. **샘플 뉴스레터**
   - 최근 발행된 뉴스레터 미리보기
   - "더 보기" 링크

5. **구독자 후기**
   - 구독자 이름과 직업
   - 후기 내용 (인용문 형식)
   - 별점 표시

6. **푸터**
   - 소셜 미디어 링크
   - 개인정보 처리방침
   - 구독 해지 안내

### CSS 스타일링
- 그라데이션 배경
- 카드 스타일 섹션
- 폼 스타일링 (포커스 효과)
- 애니메이션 효과 (fade-in, hover)
- 반응형 디자인
- **애니메이션 효과 구현:**
  - Fade-in: 페이지 로드 시 요소가 서서히 나타남
  - Hover 효과: 카드와 버튼에 부드러운 전환
  - Transform: 크기 변화, 이동, 회전 효과

### 힌트
- `background: linear-gradient()`로 그라데이션
- `box-shadow`로 카드 효과
- `::before`로 아이콘 추가
- `@media` 쿼리로 반응형 구현
- **애니메이션 예제:**
  ```css
  /* Fade-in 애니메이션 정의 */
  @keyframes fadeIn {
    from {
      opacity: 0;
      transform: translateY(20px);
    }
    to {
      opacity: 1;
      transform: translateY(0);
    }
  }
  
  /* 요소에 애니메이션 적용 */
  .hero-content {
    animation: fadeIn 1s ease-out;
  }
  
  /* Hover 효과 */
  .benefit-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(0,0,0,0.15);
    transition: all 0.3s ease;
  }
  
  /* 버튼 호버 효과 */
  .subscribe-button:hover {
    transform: scale(1.05);
    box-shadow: 0 5px 15px rgba(0,0,0,0.3);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }
  ```

### 참고 자료
- [사용자 입력](https://www.yalco.kr/@html-css/1-8)
- [인용된 콘텐츠](https://www.yalco.kr/@html-css/1-3)
- [배경 스타일링](https://www.yalco.kr/@html-css/2-8)
- [위치 지정](https://www.yalco.kr/@html-css/2-9)