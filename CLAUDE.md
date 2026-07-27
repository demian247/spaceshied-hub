# CLAUDE.md — spaceshied-hub

㈜쵸미앤세븐 SPACE SHIELD 사내 웹앱 4개를 여는 **허브**. 링크 카드만 있고 로직·DB 없음.
정적 HTML 1파일(`index.html`), 빌드 없음. `main` push → GitHub Pages 자동 배포.

## 이 repo 규칙
- **앱 링크는 `../<repo>/` 상대경로 유지.** 절대경로(`https://<owner>.github.io/...`) 금지 — 계정 이전 시 깨짐.
- **GitHub 소유자 변경은 `GH_OWNER` 상수 한 줄만** 고치면 됨(파일 상단).
- 도구 추가: `TOOLS` 배열에 한 항목 추가하면 카드 자동 생성.

## ⚙️ keep-supabase-awake 워크플로 (건드리지 말 것)
`.github/workflows/keep-supabase-awake.yml` = Supabase 무료 플랜 7일 미사용 정지를 막는 스케줄 잡.
주 3회 DB에 ping + `keepalive.txt` 하트비트 커밋(GitHub이 60일 방치 스케줄 워크플로를 끄는 것 방지).
`keepalive.txt` 는 그 하트비트 파일이니 지우지 마세요. 유료 전환 시엔 이 워크플로 삭제해도 됨.

## 전체 맥락
사내 웹앱 4개는 Supabase 프로젝트 하나(`tnuzqrqxptxrfozzjjek`)를 공유. 상세·인계 문서는
**private repo `heyjyu/spaceshied-handoff`** (README.md, DEV_IN_CLAUDE.md, apps/*.md). 접근은 오너에게 요청.
