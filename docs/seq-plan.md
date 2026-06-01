# Seq Plan — 1. 할일 입력 및 마감일 설정
생성일: 2026-06-02
상태: 진행 중

## Chunk 1 — 프로젝트 설정 + 할일 제목 입력 UI (⏳ 대기)
depends_on: 없음

- [ ] #1 [1.1.1] 할일 제목 입력 필드 UI 구현
      depends_on: 없음 / blocks: #2
      note: client(Vite+React+TS+Tailwind) + server(Express) 초기 설정 포함. paused 상태 — 이전 작업 이어서 진행.

## Chunk 2 — 할일 제목 입력값 저장 (⏳ 대기)
depends_on: Chunk 1

- [ ] #2 [1.1.2] 할일 제목 입력값 저장
      depends_on: #1 / blocks: 없음

## Chunk 3 — 마감일 캘린더 피커 + 저장 (⏳ 대기)
depends_on: Chunk 1

- [ ] #3 [1.2.1] 캘린더 피커 컴포넌트 구현
      depends_on: 없음 / blocks: #4, #5 / recommends: #1
- [ ] #4 [1.2.2] 마감일 선택 저장
      depends_on: #3 / blocks: #5

## Chunk 4 — 마감일 유효성 검사 (⏳ 대기)
depends_on: Chunk 3

- [ ] #5 [1.2.3] 마감일 유효성 검사
      depends_on: #3, #4 / blocks: 없음
