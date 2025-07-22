# 블로그 프로젝트

HTML, CSS, JavaScript, Sass를 사용한 정적 블로그 웹사이트

## 📁 프로젝트 구조

```
blog-project/
├── index.html                    # 메인 페이지
├── about.html                    # 소개 페이지
├── blog.html                     # 블로그 목록 페이지
├── post.html                     # 개별 포스트 페이지
├── assets/
│   ├── css/                      # 컴파일된 CSS
│   ├── scss/                     # Sass 소스 파일
│   ├── js/                       # JavaScript 파일
│   ├── images/                   # 이미지 파일
│   └── fonts/                    # 웹폰트 파일
├── data/                         # JSON 데이터 파일
├── wiki/                         # 개발 가이드라인
└── .github/                      # GitHub 템플릿
```

## 🚀 시작하기

### 로컬 개발 환경 설정

1. **저장소 클론**
   ```bash
   git clone https://github.com/MinKyeongHyeon/coworkTest.git
   cd coworkTest
   ```

2. **Sass 컴파일 설정** (선택사항)
   ```bash
   # Node.js가 설치되어 있다면
   npm install -g sass
   sass --watch assets/scss:assets/css
   ```

3. **라이브 서버 실행**
   - VS Code Live Server 확장 사용
   - 또는 Python 간단 서버: `python -m http.server 8000`

## 📚 개발 가이드라인

우리 팀의 개발 가이드라인은 [Wiki](./wiki/)에서 확인할 수 있습니다:

- 📝 [코드 컨벤션 가이드](./wiki/코드-컨벤션-가이드.md)
- 🔄 [커밋 컨벤션 가이드](./wiki/커밋-컨벤션-가이드.md)  
- 🔍 [PR 템플릿과 사용법](./wiki/PR-템플릿과-사용법.md)

## 🤝 기여하기

1. 이슈를 생성하여 작업 내용을 공유해주세요
2. 브랜치 명명 규칙을 따라 작업 브랜치를 생성해주세요
3. 코드 컨벤션을 준수하여 개발해주세요
4. PR 템플릿을 사용하여 Pull Request를 생성해주세요

## 🔧 기술 스택

- **HTML5**: 시맨틱 마크업
- **CSS3**: Flexbox, Grid 레이아웃
- **Sass/SCSS**: CSS 전처리기
- **JavaScript (ES6+)**: 모던 자바스크립트
- **반응형 디자인**: 모바일 퍼스트 접근

## 📞 팀 정보

- **팀 구성**: 프론트엔드 개발자 4명
- **프로젝트 목표**: 반응형 블로그 웹사이트 개발
- **개발 기간**: 진행 중

## 📄 라이선스

This project is licensed under the MIT License.
