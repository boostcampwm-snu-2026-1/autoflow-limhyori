# .claude/commands/config-sync.md

chore/claude-config 브랜치 작업 전 dev 최신화.

Claude 설정 파일(.claude/)을 수정하려는데 chore/claude-config가 dev보다 오래됐을 때 사용.

실행 순서:
```bash
# 1. 현재 변경사항 임시 저장 (있으면)
git stash

# 2. dev 최신화
git checkout dev
git pull origin dev

# 3. chore/claude-config로 전환 후 dev 기준 rebase
git checkout chore/claude-config
git rebase dev
```

충돌 발생 시:
- 충돌 파일 목록 표시
- "충돌을 해결하고 `git rebase --continue` 를 실행해주세요." 안내

완료 후:
```bash
git stash pop  # 저장한 변경사항 복원 (있으면)
```

출력:
```
✅ chore/claude-config가 dev 기준으로 최신화됐습니다.
현재 브랜치: chore/claude-config
```
