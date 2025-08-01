# 💡 FAQ 페이지 만들기

자주 묻는 질문(FAQ) 페이지를 만들어봅시다. 아코디언 스타일로 질문을 클릭하면 답변이 펼쳐지는 인터랙티브한 디자인을 구현해야 합니다.

## 요구사항

### HTML 구조
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>고객 지원 - FAQ</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- 여기에 코드 작성 -->
</body>
</html>
```

### 필요한 요소들

1. **헤더 영역**
   - 페이지 제목: `<h1>` "자주 묻는 질문"
   - 설명: `<p>` "고객님들이 자주 문의하시는 내용을 정리했습니다"

2. **검색 바**
   - 검색 입력 필드
   - 검색 버튼

3. **카테고리 탭**
   - 전체, 계정, 결제, 배송, 환불
   - `<nav>`와 리스트로 구성

4. **FAQ 아이템** (최소 8개)
   - 각 항목은 `<details>`와 `<summary>` 태그 사용
   - 질문: `<summary>` 태그
   - 답변: `<p>` 태그로 상세 내용
   - 카테고리 표시

5. **추가 도움말 섹션**
   - 문의하기 버튼
   - 고객센터 정보

### 예시 FAQ 항목
- 회원가입은 어떻게 하나요?
- 비밀번호를 잊어버렸어요
- 주문 취소는 어떻게 하나요?
- 배송 기간은 얼마나 걸리나요?
- 환불 정책이 어떻게 되나요?
- 포인트는 어떻게 사용하나요?
- 해외 배송이 가능한가요?
- 회원 탈퇴는 어떻게 하나요?

### CSS 스타일링
- 아코디언 효과 (클릭 시 열림/닫힘)
- 카테고리별 색상 구분
- 호버 효과
- 부드러운 전환 효과
- 검색 바 스타일

### 힌트
- `<details>`와 `<summary>` 태그는 기본 아코디언 기능 제공
- `details[open]` 선택자로 열린 상태 스타일링
- `::marker` 가상 요소로 화살표 커스터마이징
- `transition`으로 부드러운 애니메이션

### 참고 자료
- [용도와 중요도별 태그](https://www.yalco.kr/@html-css/1-2)
- [목록으로 나열하기](https://www.yalco.kr/@html-css/1-4)
- [요소 숨기기](https://www.yalco.kr/@html-css/2-10)