# VAR - 한글 변수명 생성기

[![GitHub Pages](https://img.shields.io/badge/GitHub-Pages-green)](https://your-username.github.io/var-generator)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Korean](https://img.shields.io/badge/Language-Korean-blue)](https://github.com/your-username/var-generator)

> 🚀 **200+ 단어 지원, 완전 오프라인 동작하는 한글 변수명 생성기**

한글 단어를 영문 변수명으로 변환해주는 개발자 도구입니다. 네트워크 연결 없이도 완벽하게 동작하며, 3가지 알고리즘으로 다양한 네이밍 옵션을 제공합니다.

## ✨ 주요 기능

### 🎯 3가지 알고리즘 엔진
- **Juno**: 직역 알고리즘 - 한글을 직접적으로 영어로 번역
- **Indigo**: 문맥 알고리즘 - 맥락을 고려한 다양한 동의어 제공  
- **Kepler**: 약어 알고리즘 - 짧고 간결한 약어 형태 추천

### 📚 포괄적 단어 지원
- **200+ 한글 단어** 매핑 데이터
- **비즈니스 용어**: 회원, 고객, 상품, 주문, 결제, 배송...
- **기술 용어**: 데이터베이스, 서버, 클라이언트, API, 세션...
- **일반 동작**: 등록, 수정, 삭제, 조회, 검색, 생성, 저장...

### 🧠 지능형 복합어 처리
- 자동 단어 분해: `회원관리` → `회원` + `관리`
- 스마트 조합: `member` + `management` → `memberManagement`
- 2-3단어 복합어까지 완벽 지원

### 🔧 접두사/접미사 자동 추가
- **접두사**: get, set, create, update, delete, find, check, is, has
- **접미사**: List, Info, Data, Count, Status, Manager, Service
- 원클릭으로 모든 결과에 일괄 적용

### 📱 반응형 디자인
- 모바일, 태블릿, PC 모든 화면 최적화
- 사이버네틱 다크 테마
- 부드러운 애니메이션 효과

## 🚀 사용법

### 1. 기본 사용
```
입력: 사용자
결과: 
- camelCase: user
- snake_case: user  
- PascalCase: User
- kebab-case: user
```

### 2. 복합어 처리
```
입력: 회원관리
결과:
- camelCase: memberManagement
- snake_case: member_management
- PascalCase: MemberManagement  
- kebab-case: member-management
```

### 3. 접두사 추가
```
"데이터" + "get" 클릭
→ getData, get_data, GetData, get-data
```

## 🛠 설치 및 배포

### GitHub Pages 배포

1. **저장소 생성**
```bash
# 새 저장소 생성
git init var-generator
cd var-generator

# 파일 복사
# index.html, style.css, app.js, README.md를 복사

# Git 설정
git add .
git commit -m "Initial commit: VAR Generator"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/var-generator.git
git push -u origin main
```

2. **GitHub Pages 활성화**
- GitHub 저장소 → Settings → Pages
- Source: Deploy from a branch
- Branch: main / (root)  
- Save 클릭

3. **접속**
- `https://YOUR_USERNAME.github.io/var-generator`

### 로컬 실행

```bash
# 파일 다운로드
git clone https://github.com/YOUR_USERNAME/var-generator.git
cd var-generator

# 로컬 서버 실행 (Python)
python -m http.server 8000

# 또는 Node.js
npx serve .

# 브라우저에서 접속
open http://localhost:8000
```

## 📁 파일 구조

```
var-generator/
├── index.html          # 메인 HTML 파일  
├── style.css           # CSS 스타일시트
├── app.js              # JavaScript 로직
└── README.md           # 프로젝트 문서
```

## 🎨 커스터마이징

### 색상 테마 변경

`style.css`에서 CSS 변수 수정:

```css
:root {
  --color-accent-cyan: #00d4d4;    /* 메인 강조색 */
  --color-accent-green: #39ff39;   /* 보조 강조색 */
  --color-bg-primary: #1a1f2e;     /* 배경색 */
}
```

### 사전 단어 추가

`app.js`의 `dictionary` 객체에 새 단어 추가:

```javascript
this.dictionary = {
  // 기존 단어들...
  "새단어": ["newword", "fresh", "novel", "recent"],
  "맞춤단어": ["custom", "personalized", "tailored"]
};
```

## 🔧 기술 스택

- **HTML5**: 시맨틱 마크업
- **CSS3**: Flexbox, Grid, CSS Variables
- **Vanilla JavaScript**: ES6+, 완전 의존성 없음
- **Local Storage**: 히스토리 저장
- **완전 오프라인**: 외부 API 의존성 없음

## 📊 지원 단어 예시

| 분류 | 한글 | 영어 옵션 |
|------|------|-----------|
| 사용자 | 회원 | member, user, subscriber, account |
| 전자상거래 | 상품 | product, item, goods, merchandise |
| 데이터 | 목록 | list, array, collection, items |
| 작업 | 검색 | search, find, query, lookup |
| 상태 | 활성 | active, enabled, live |

## 🤝 기여하기

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### 기여 아이디어
- 새로운 한글 단어 추가
- 번역 품질 개선  
- 새로운 네이밍 컨벤션 지원
- UI/UX 개선
- 접근성 향상

## 📝 라이선스

이 프로젝트는 MIT 라이선스로 배포됩니다. 자세한 내용은 [LICENSE](LICENSE) 파일을 참조하세요.

## 🙏 감사의 말

- 개발자 커뮤니티의 피드백
- 오픈소스 한글 처리 라이브러리들
- GitHub Pages 무료 호스팅

## 📞 연락처

프로젝트 링크: [https://github.com/YOUR_USERNAME/var-generator](https://github.com/YOUR_USERNAME/var-generator)

---

⭐ 이 프로젝트가 도움이 되었다면 스타를 눌러주세요!

> **개발자를 위한, 개발자에 의한 완전 무료 도구** 🚀
