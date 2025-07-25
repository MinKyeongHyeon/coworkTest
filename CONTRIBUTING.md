# 기여 가이드

이 프로젝트에 기여해 주셔서 감사합니다! 🎉

## 📋 기여하기 전에 읽어주세요

### 필수 문서
- [코드 컨벤션 가이드](./wiki/코드-컨벤션-가이드.md)
- [커밋 컨벤션 가이드](./wiki/커밋-컨벤션-가이드.md)
- [PR 템플릿과 사용법](./wiki/PR-템플릿과-사용법.md)

## 🚀 기여 프로세스

### 1. 이슈 생성
```markdown
새로운 기능이나 버그 수정을 시작하기 전에 GitHub Issue를 생성해주세요.
- 기능 요청: Feature Request 템플릿 사용
- 버그 리포트: Bug Report 템플릿 사용
```

### 2. 브랜치 생성
```bash
# main 브랜치에서 최신 코드 가져오기
git checkout main
git pull origin main

# 새 브랜치 생성 (이슈 번호 포함 권장)
git checkout -b feature/123-blog-search-functionality
git checkout -b bugfix/456-mobile-navigation-fix
```

### 3. 개발 작업
- **코드 컨벤션** 준수
- **커밋 컨벤션** 준수
- **테스트** 수행
- **문서** 업데이트 (필요시)

### 4. Pull Request 생성
- PR 템플릿을 사용해서 상세히 작성
- 관련 이슈 번호 연결
- 스크린샷 첨부 (UI 변경시)
- 적절한 리뷰어 지정

### 5. 코드 리뷰
- 리뷰어의 피드백에 적극적으로 대응
- 변경사항을 명확히 설명
- 필요시 추가 커밋 또는 수정

### 6. 머지
- 모든 리뷰가 완료되고 승인되면 머지
- 머지 후 브랜치 삭제

## 🎯 코드 품질 가이드라인

### HTML
- 시맨틱 태그 사용
- 접근성 고려 (ARIA 라벨, alt 텍스트 등)
- BEM 방법론 클래스명 사용

### CSS/Sass
- 모바일 퍼스트 접근
- 재사용 가능한 컴포넌트 설계
- 성능 최적화 고려

### JavaScript
- ES6+ 문법 사용
- 함수형 프로그래밍 지향
- 에러 핸들링 구현
- 명확한 함수/변수명 사용

## 🧪 테스트 가이드라인

### 필수 테스트
- [ ] 데스크톱 브라우저 (Chrome, Firefox, Safari)
- [ ] 모바일 브라우저 (iOS Safari, Android Chrome)
- [ ] 반응형 디자인 (320px ~ 1920px)
- [ ] 접근성 테스트 (키보드 네비게이션, 스크린 리더)

### 성능 테스트
- [ ] 페이지 로딩 속도
- [ ] 이미지 최적화
- [ ] CSS/JS 번들 크기
- [ ] Lighthouse 점수 확인

## 📝 문서화 가이드라인

### 코드 주석
```javascript
/**
 * 블로그 포스트를 필터링합니다.
 * @param {Array} posts - 블로그 포스트 배열
 * @param {string} category - 필터링할 카테고리
 * @returns {Array} 필터링된 포스트 배열
 */
function filterPostsByCategory(posts, category) {
    return posts.filter(post => post.category === category);
}
```

### README 업데이트
새로운 기능을 추가하거나 설정이 변경되면 README.md를 업데이트해주세요.

### Wiki 업데이트
팀 전체에 영향을 주는 컨벤션 변경사항은 Wiki에 반영해주세요.

## 🔍 코드 리뷰 가이드라인

### 리뷰 요청자
- PR 설명을 상세히 작성
- 변경사항에 대한 컨텍스트 제공
- 테스트 완료 여부 명시
- 스크린샷 또는 GIF 첨부 (UI 변경시)

### 리뷰어
- 건설적인 피드백 제공
- 코드의 좋은 점도 언급
- 구체적인 개선 방안 제시
- 질문이나 제안사항 명확히 표현

## 🚨 주의사항

### 하지 말아야 할 것들
- ❌ main 브랜치에 직접 커밋
- ❌ 테스트 없이 PR 생성
- ❌ 컨벤션 무시
- ❌ 다른 기능과 관련없는 변경사항 포함
- ❌ 대용량 파일 커밋 (이미지는 압축 후 커밋)

### 권장사항
- ✅ 작고 집중된 PR 생성
- ✅ 명확한 커밋 메시지 작성
- ✅ 코드 리뷰에 적극적으로 참여
- ✅ 문제 발생시 팀원과 소통
- ✅ 새로운 아이디어나 개선사항 제안

## 💬 소통 채널

### 질문이나 도움이 필요할 때
1. **GitHub Issues**: 버그 리포트, 기능 요청
2. **GitHub Discussions**: 일반적인 질문, 토론
3. **PR Comments**: 코드 리뷰 관련 논의
4. **팀 미팅**: 중요한 의사결정 사항

### 응답 시간
- **일반 질문**: 24시간 이내
- **긴급 버그**: 4시간 이내
- **코드 리뷰**: 48시간 이내

## 🎉 기여 인정

모든 기여자는 README의 Contributors 섹션에 추가됩니다.
특별한 기여를 해주신 분들은 별도로 감사 인사를 드립니다.

## 📄 라이선스

이 프로젝트에 기여함으로써 MIT 라이선스 하에 공개됨에 동의하는 것으로 간주됩니다.

---

다시 한 번 기여해 주셔서 감사합니다! 함께 훌륭한 블로그 프로젝트를 만들어가요! 🚀
