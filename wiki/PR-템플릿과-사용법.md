# Pull Request 템플릿과 사용법

> 효율적인 코드 리뷰와 협업을 위한 PR 템플릿과 가이드라인입니다.

## 기능 개발용 PR 템플릿

### 템플릿 생성 방법
GitHub에서 `.github/pull_request_template.md` 파일을 생성하면 자동으로 적용됩니다.

```markdown
## 📝 개요
<!-- 이 PR에서 구현한 기능이나 변경사항을 간단히 설명해주세요 -->

## 🔗 관련 이슈
<!-- 관련된 이슈 번호를 적어주세요 -->
- Closes #이슈번호
- Related to #이슈번호

## ✨ 변경사항
<!-- 구체적인 변경사항을 체크리스트로 작성해주세요 -->
- [ ] 새로운 기능 추가
- [ ] UI/UX 개선
- [ ] 성능 최적화
- [ ] 코드 리팩토링
- [ ] 문서 업데이트

### 📋 상세 변경사항
<!-- 변경사항을 자세히 설명해주세요 -->
1. **기능 A 추가**
   - 설명...
   
2. **컴포넌트 B 수정**
   - 설명...

## 🧪 테스트
<!-- 테스트한 내용을 체크해주세요 -->
- [ ] 데스크톱 브라우저 테스트 (Chrome, Firefox, Safari)
- [ ] 모바일 브라우저 테스트
- [ ] 반응형 디자인 확인
- [ ] 접근성 확인
- [ ] 성능 테스트

### 테스트 시나리오
<!-- 구체적인 테스트 시나리오를 작성해주세요 -->
1. **테스트 케이스 1**
   - 단계: ...
   - 예상 결과: ...
   
2. **테스트 케이스 2**
   - 단계: ...
   - 예상 결과: ...

## 📱 스크린샷/GIF
<!-- 변경사항을 시각적으로 보여주는 스크린샷이나 GIF를 첨부해주세요 -->

### Before (변경 전)
![Before](링크)

### After (변경 후)
![After](링크)

## 🎯 리뷰 포인트
<!-- 리뷰어가 특별히 확인해야 할 부분이 있다면 명시해주세요 -->
- [ ] 코드 구조 및 설계
- [ ] 성능 영향도
- [ ] 보안 고려사항
- [ ] 브라우저 호환성
- [ ] 접근성 준수

## 🔄 배포 고려사항
<!-- 배포 시 고려해야 할 사항이 있다면 적어주세요 -->
- [ ] 데이터베이스 마이그레이션 필요
- [ ] 환경 변수 추가/수정 필요
- [ ] 캐시 초기화 필요
- [ ] 특별한 배포 순서 필요

## 📚 참고 자료
<!-- 참고한 문서, 디자인, API 문서 등의 링크를 첨부해주세요 -->
- [디자인 시안](링크)
- [API 문서](링크)
- [참고 문서](링크)

---

## 체크리스트
- [ ] 코드 컨벤션을 준수했습니다
- [ ] 커밋 메시지를 규칙에 맞게 작성했습니다
- [ ] 관련 문서를 업데이트했습니다
- [ ] 충분한 테스트를 완료했습니다
- [ ] 리뷰어를 지정했습니다
```

---

## 버그 수정용 PR 템플릿

```markdown
## 🐛 버그 수정 개요
<!-- 수정한 버그에 대해 간단히 설명해주세요 -->

## 🔗 관련 이슈
- Fixes #이슈번호

## 🎯 버그 상황
### 문제 상황
<!-- 버그가 발생한 상황을 구체적으로 설명해주세요 -->

### 재현 방법
1. 단계 1
2. 단계 2  
3. 단계 3

### 예상 동작
<!-- 정상적으로 동작해야 하는 방식을 설명해주세요 -->

### 실제 동작
<!-- 실제로 발생한 문제를 설명해주세요 -->

## 🔧 해결 방법
<!-- 어떻게 문제를 해결했는지 설명해주세요 -->

### 근본 원인
<!-- 버그의 근본 원인을 분석해주세요 -->

### 수정 내용
1. **파일 A 수정**
   - 수정 내용...
   
2. **파일 B 수정**
   - 수정 내용...

## 🧪 테스트 및 검증
- [ ] 원본 버그 재현 불가능 확인
- [ ] 관련 기능 정상 동작 확인
- [ ] 회귀 테스트 완료
- [ ] 다양한 브라우저에서 테스트 완료

### 테스트 케이스
1. **정상 케이스 테스트**
   - 단계: ...
   - 결과: ✅ 성공
   
2. **경계 케이스 테스트**
   - 단계: ...
   - 결과: ✅ 성공

## 📊 영향 범위
<!-- 이 수정이 다른 기능에 미칠 수 있는 영향을 분석해주세요 -->
- [ ] 영향 없음
- [ ] 제한적 영향 (상세 설명 필요)
- [ ] 광범위한 영향 (상세 설명 필요)

## 🔄 추가 고려사항
- [ ] 유사한 버그가 다른 곳에도 있는지 확인
- [ ] 모니터링 추가 필요
- [ ] 사용자 알림 필요

---

## 체크리스트
- [ ] 버그 수정을 완료했습니다
- [ ] 관련 테스트를 모두 통과했습니다  
- [ ] 코드 리뷰를 요청했습니다
- [ ] 문서를 업데이트했습니다 (필요시)
```

---

## PR 리뷰 가이드라인

### 리뷰어 가이드

#### 1. 리뷰 시 확인 사항
```markdown
## 📋 코드 리뷰 체크리스트

### 기능성
- [ ] 요구사항을 제대로 구현했는가?
- [ ] 예외 상황을 적절히 처리했는가?
- [ ] 성능에 문제가 없는가?

### 코드 품질
- [ ] 코드 컨벤션을 따르고 있는가?
- [ ] 함수/변수명이 명확한가?
- [ ] 중복 코드가 없는가?
- [ ] 주석이 적절한가?

### 보안성
- [ ] 보안 취약점이 없는가?
- [ ] 입력값 검증을 하고 있는가?
- [ ] 민감한 정보가 노출되지 않는가?

### 호환성
- [ ] 브라우저 호환성을 고려했는가?
- [ ] 모바일에서 정상 동작하는가?
- [ ] 접근성을 고려했는가?
```

#### 2. 리뷰 댓글 작성 방법

##### ✅ 좋은 리뷰 댓글 예시
```markdown
# 🎯 개선 제안
이 부분에서 성능 개선이 가능할 것 같습니다.

**현재 코드:**
```javascript
const filteredPosts = posts.filter(post => post.category === category);
```

**제안:**
```javascript
// 카테고리별 인덱싱을 통한 성능 최적화
const filteredPosts = categoryIndex[category] || [];
```

**이유:** 매번 전체 배열을 순회하는 대신 미리 인덱싱된 데이터를 사용하면 성능이 향상됩니다.

# ✨ 칭찬
반응형 디자인 구현이 정말 깔끔하네요! 브레이크포인트 관리도 체계적으로 잘 하셨습니다.

# ❓ 질문
이 부분에서 `setTimeout`을 사용한 특별한 이유가 있나요? `requestAnimationFrame`을 사용하는 것이 더 적절할 것 같은데 어떻게 생각하시나요?

# 🐛 버그 발견
mobile 환경에서 이 버튼이 클릭되지 않을 수 있습니다.

**문제:** `touch-action` 속성이 누락되어 터치 이벤트가 제대로 처리되지 않을 수 있습니다.
**해결방법:** CSS에 `touch-action: manipulation;` 추가
```

##### ❌ 피해야 할 리뷰 댓글
```markdown
# 너무 모호한 피드백
이 코드는 별로다.
좀 더 좋게 해주세요.

# 너무 공격적인 표현  
이런 식으로 코딩하면 안 됩니다.
왜 이렇게 복잡하게 했나요?

# 구체적인 대안 없는 비판
이 방법은 좋지 않습니다.
성능이 안 좋을 것 같습니다.
```

#### 3. 리뷰 승인 기준
```markdown
## ✅ 승인 (Approve)
- 모든 요구사항이 구현됨
- 코드 품질이 팀 기준을 만족
- 테스트가 충분히 완료됨
- 문서가 적절히 업데이트됨

## 🔄 변경 요청 (Request Changes)
- 기능상 문제가 있음
- 보안/성능에 심각한 문제가 있음
- 코드 컨벤션을 현저히 위반함

## 💬 의견 (Comment)  
- 사소한 개선사항 제안
- 질문이나 토론거리 제공
- 칭찬이나 학습 포인트 공유
```

### PR 작성자 가이드

#### 1. PR 작성 전 준비사항
```bash
# 1. 최신 main 브랜치와 동기화
git checkout main
git pull origin main
git checkout feature/your-feature
git rebase main

# 2. 코드 스타일 검사
npm run lint  # 또는 해당 프로젝트의 린팅 도구

# 3. 테스트 실행
npm test  # 또는 해당 프로젝트의 테스트 명령어

# 4. 변경사항 재확인
git diff main...HEAD
```

#### 2. PR 설명 작성 팁
```markdown
# ✅ 좋은 PR 설명
## 배경
사용자들이 블로그 포스트를 빠르게 찾을 수 있도록 검색 기능이 필요했습니다.

## 구현 방법
1. 검색 입력 컴포넌트 구현
2. 실시간 검색 필터링 로직 추가
3. 검색 결과 하이라이팅 기능 구현

## 주요 변경사항
- `SearchComponent.js`: 검색 입력 및 UI 컴포넌트
- `searchUtils.js`: 검색 알고리즘 및 필터링 로직
- `blog.css`: 검색 결과 스타일링

# ❌ 나쁜 PR 설명
검색 기능 추가했습니다.
```

#### 3. 코드 리뷰 대응 방법
```markdown
# ✅ 좋은 대응
감사합니다! 말씀해주신 부분 수정했습니다.

**변경사항:**
- `debounce` 함수를 사용해서 성능 최적화
- 에러 핸들링 로직 추가
- 접근성을 위한 ARIA 라벨 추가

새로운 커밋: abc1234

# ❌ 나쁜 대응
네, 수정했습니다.
(구체적인 설명 없음)
```

---

## PR 크기 제한 가이드

### 1. 적정 PR 크기 기준
```markdown
## 🟢 이상적인 크기 (추천)
- **변경된 파일**: 5개 이하
- **변경된 라인**: 200라인 이하  
- **리뷰 시간**: 30분 이하
- **커밋 개수**: 3개 이하

## 🟡 보통 크기 (허용)
- **변경된 파일**: 10개 이하
- **변경된 라인**: 500라인 이하
- **리뷰 시간**: 1시간 이하
- **커밋 개수**: 5개 이하

## 🔴 큰 크기 (분할 고려)
- **변경된 파일**: 10개 초과
- **변경된 라인**: 500라인 초과
- **리뷰 시간**: 1시간 초과
- **커밋 개수**: 5개 초과
```

### 2. 큰 PR을 나누는 방법

#### 예시: 블로그 검색 기능 구현
```markdown
# ❌ 큰 PR (나쁜 예)
feat: implement complete blog search functionality

- Add search input component
- Add search result component  
- Add search API integration
- Add search result highlighting
- Add search history
- Add search analytics
- Update navigation to include search
- Add responsive design for search
- Add search performance optimization
- Update documentation

# ✅ 작은 PR들로 분할 (좋은 예)

## PR 1: feat: add basic search input component
- Search input UI component
- Basic validation logic
- CSS styling

## PR 2: feat: implement search filtering logic  
- Search algorithm implementation
- Filter functions
- Unit tests

## PR 3: feat: add search result display
- Search result component
- Result highlighting
- Pagination

## PR 4: feat: integrate search with navigation
- Navigation menu updates
- Responsive design
- User experience improvements
```

### 3. PR 분할 전략

#### 기능별 분할
```markdown
1. **UI 컴포넌트** → 별도 PR
2. **비즈니스 로직** → 별도 PR  
3. **API 연동** → 별도 PR
4. **스타일링** → 별도 PR
5. **테스트** → 별도 PR
```

#### 레이어별 분할
```markdown
1. **데이터 레이어** → 별도 PR
2. **서비스 레이어** → 별도 PR
3. **UI 레이어** → 별도 PR
4. **통합** → 별도 PR
```

### 4. 예외적으로 큰 PR이 허용되는 경우
```markdown
## 🎯 허용되는 큰 PR
- **자동 생성 코드** (코드 생성기, 컴파일러 출력)
- **라이브러리 업데이트** (package-lock.json 등)
- **파일 이동/이름 변경** (리팩토링)
- **데이터 마이그레이션**
- **긴급 핫픽스** (여러 파일에 걸친 긴급 수정)

이런 경우에도 가능하면 논리적으로 분할을 시도해주세요.
```

---

## PR 체크리스트 템플릿

### 작성자용 체크리스트
```markdown
## 📝 PR 작성 전 체크리스트

### 코드 품질
- [ ] 코딩 컨벤션을 준수했습니다
- [ ] 의미있는 함수/변수명을 사용했습니다
- [ ] 주석을 적절히 작성했습니다
- [ ] 불필요한 코드를 제거했습니다

### 기능성
- [ ] 요구사항을 모두 구현했습니다
- [ ] 예외 상황을 고려했습니다
- [ ] 입력 검증을 구현했습니다

### 테스트
- [ ] 데스크톱에서 테스트했습니다
- [ ] 모바일에서 테스트했습니다  
- [ ] 여러 브라우저에서 테스트했습니다
- [ ] 접근성을 확인했습니다

### 문서화
- [ ] README를 업데이트했습니다 (필요시)
- [ ] 코멘트를 업데이트했습니다
- [ ] 관련 이슈를 연결했습니다

### 리뷰
- [ ] 적절한 리뷰어를 지정했습니다
- [ ] PR 설명을 상세히 작성했습니다
- [ ] 스크린샷을 첨부했습니다 (UI 변경시)
```

### 리뷰어용 체크리스트
```markdown
## 🔍 리뷰어 체크리스트

### 기능 검토
- [ ] 요구사항이 제대로 구현되었나요?
- [ ] 예외 처리가 적절한가요?
- [ ] 사용자 경험이 향상되었나요?

### 코드 품질
- [ ] 코드가 읽기 쉬운가요?
- [ ] 중복 코드가 없나요?
- [ ] 함수가 단일 책임을 가지고 있나요?

### 성능 및 보안
- [ ] 성능에 부정적인 영향이 없나요?
- [ ] 보안 취약점이 없나요?
- [ ] 메모리 누수 가능성이 없나요?

### 호환성
- [ ] 브라우저 호환성이 고려되었나요?
- [ ] 반응형 디자인이 적용되었나요?
- [ ] 접근성이 고려되었나요?

### 리뷰 완료
- [ ] 건설적인 피드백을 제공했습니다
- [ ] 개선점을 구체적으로 제시했습니다
- [ ] 좋은 점도 언급했습니다
```

이 가이드를 통해 효율적이고 협력적인 코드 리뷰 문화를 만들어가세요! 처음에는 복잡해 보일 수 있지만, 익숙해지면 코드 품질과 팀워크가 크게 향상될 거예요! 🚀
