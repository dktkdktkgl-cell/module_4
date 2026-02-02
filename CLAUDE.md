# Claude AI 활용 가이드

## 프로젝트 개요
이 프로젝트는 Claude AI를 활용하여 개발되고 있습니다.

## Claude를 활용한 개발 프로세스

### 1. 코드 작성 및 리팩토링
- Claude Code를 통한 효율적인 코드 작성
- 코드 리뷰 및 개선 제안
- 베스트 프랙티스 적용

### 2. 문서화
- 프로젝트 문서 자동 생성
- README 및 가이드 작성
- API 문서화

### 3. 디버깅 및 문제 해결
- 버그 분석 및 수정
- 성능 최적화 제안
- 에러 해결 가이드

## Claude 사용 팁

### 효과적인 프롬프트 작성
```
- 구체적이고 명확한 요청
- 필요한 컨텍스트 제공
- 단계별 작업 분할
```

### 코드 리뷰 요청 예시
```
이 함수의 성능을 개선할 수 있는 방법을 제안해주세요.
보안 취약점이 있는지 검토해주세요.
코드의 가독성을 높일 수 있는 방법을 알려주세요.
```

## 개발 워크플로우

1. **계획 수립** - `docs/plan.md` 참조
2. **개발 진행** - Claude Code와 함께 작업
3. **진행 상황 기록** - `docs/progress.md` 업데이트
4. **코드 리뷰** - Claude를 통한 코드 품질 검증
5. **문서화** - 자동화된 문서 생성 및 업데이트

## 유용한 Claude 명령어

### 파일 작업
- 파일 읽기 및 분석
- 코드 수정 및 리팩토링
- 새 파일 생성

### Git 작업
- 커밋 메시지 작성
- PR 생성 및 관리
- 코드 변경 사항 검토

### 프로젝트 관리
- 작업 목록 관리
- 진행 상황 추적
- 이슈 해결

## Custom Skills

이 프로젝트는 `.claude/skills/` 폴더에 커스텀 skills를 정의하여 반복적인 작업을 자동화합니다.

### 사용 가능한 Skills

#### `/git-commit`
Git 커밋 프로세스를 자동화하는 skill입니다.

**실행 순서:**
1. `docs/plan.md`와 `docs/progress.md` 최신화
   - 체크박스 업데이트
2. 변경된 파일들을 git add
   - 현재 세션에서 수정된 파일만 추가
3. 커밋 메시지 작성
   - Git/Branch 전략에 따라 상세하게 작성
4. Git push 수행

**사용 방법:**
```
/git-commit
```

### Skills 추가 방법

새로운 skill을 추가하려면:
1. `.claude/skills/` 폴더에 새 디렉토리 생성
2. `SKILL.md` 파일 작성
3. Frontmatter에 name과 description 정의
4. 실행할 작업 내용 작성

**예시 구조:**
```
.claude/skills/
└── your-skill-name/
    └── SKILL.md
```

## 참고 자료
- [Claude AI 공식 문서](https://docs.anthropic.com/)
- [Claude Code GitHub](https://github.com/anthropics/claude-code)
- 프로젝트 문서: `docs/` 폴더 참조

## 기여 방법
Claude를 활용하여 프로젝트에 기여할 때는:
1. 변경 사항을 명확히 설명
2. 코드 품질 유지
3. 문서 업데이트
4. 테스트 작성

---
*이 문서는 Claude AI와 함께 작성되었습니다.*
