# CLAUDE.md — spaceshied-hub

㈜쵸미앤세븐 SPACE SHIELD 사내 웹앱 4개를 여는 **허브**. 링크 카드만 있고 로직·DB 없음.
정적 HTML 1파일(`index.html`), 빌드 없음. `main` push → GitHub Pages 자동 배포.

## 이 repo 규칙
- **앱 링크는 `../<repo>/` 상대경로 유지.** 절대경로(`https://<owner>.github.io/...`) 금지 — 계정 이전 시 깨짐.
- **GitHub 소유자 변경은 `GH_OWNER` 상수 한 줄만** 고치면 됨(파일 상단).
- 도구 추가: `TOOLS` 배열에 한 항목 추가하면 카드 자동 생성.

## 전체 맥락
사내 웹앱 4개는 Supabase 프로젝트 하나(`tnuzqrqxptxrfozzjjek`)를 공유. 상세·인계 문서는
**private repo `heyjyu/spaceshied-handoff`** (README.md, DEV_IN_CLAUDE.md, apps/*.md). 접근은 오너에게 요청.
