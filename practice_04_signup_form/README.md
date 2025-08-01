# 💡 회원가입 폼 만들기

사용자 친화적인 회원가입 폼을 만들어봅시다. 다양한 입력 타입과 유효성 검사를 포함해야 합니다.

## 요구사항

### HTML 구조
```html
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>회원가입</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- 여기에 코드 작성 -->
</body>
</html>
```

### 필요한 요소들

1. **폼 컨테이너**
   - `<form>` 태그 사용
   - `autocomplete="off"` 속성 추가

2. **기본 정보 섹션** (`<fieldset>`과 `<legend>` 사용)
   - 아이디: `type="text"`, `required`, `minlength="4"`
   - 비밀번호: `type="password"`, `required`, `minlength="8"`
   - 비밀번호 확인: `type="password"`, `required`
   - 이메일: `type="email"`, `required`

3. **개인 정보 섹션** (`<fieldset>`과 `<legend>` 사용)
   - 이름: `type="text"`, `required`
   - 생년월일: `type="date"`, `required`
   - 성별: `type="radio"` (남성/여성/기타)
   - 전화번호: `type="tel"`, `pattern="[0-9]{3}-[0-9]{4}-[0-9]{4}"`

4. **추가 정보 섹션**
   - 관심사: `type="checkbox"` (IT, 디자인, 마케팅, 기타)
   - 자기소개: `<textarea>`, `rows="5"`

5. **약관 동의**
   - 전체 동의: `type="checkbox"`
   - 이용약관 동의: `type="checkbox"`, `required`
   - 개인정보 처리방침 동의: `type="checkbox"`, `required`

6. **버튼**
   - 가입하기: `type="submit"`
   - 초기화: `type="reset"`

### CSS 스타일링
- 폼 최대 너비: 500px, 중앙 정렬
- `fieldset` 간격과 테두리 스타일
- 입력 필드 100% 너비
- 포커스 상태 스타일 변경
- 버튼 호버 효과

### 힌트
- 각 입력 필드에는 `<label>` 태그 필수
- `for` 속성으로 라벨과 입력 필드 연결
- `placeholder` 속성으로 입력 힌트 제공
- `:focus` 선택자로 포커스 스타일 적용

### 참고 자료
- [사용자 입력 1](https://www.yalco.kr/@html-css/1-8)
- [사용자 입력 2](https://www.yalco.kr/@html-css/1-9)
- [사용자 입력 3](https://www.yalco.kr/@html-css/1-10)