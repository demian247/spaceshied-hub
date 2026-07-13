# spaceshied-hub

스페이스쉴드 통합 **회사 관리 허브(포털)**. 흩어진 관리 도구들을 한 페이지에서 링크로 묶는다.

**라이브**: https://heyjyu.github.io/spaceshied-hub/

## 연결된 도구

| # | 도구 | 라이브 | Repo |
|---|------|--------|------|
| 01 | 쿠팡 상품 관리 | https://heyjyu.github.io/coupang-ops/ | [coupang-ops](https://github.com/heyjyu/coupang-ops) |
| 02 | 포장 운영 관리 | https://heyjyu.github.io/spaceshield-packaging/ | [spaceshield-packaging](https://github.com/heyjyu/spaceshield-packaging) |
| 03 | 상품 카테고리 | https://heyjyu.github.io/spaceshied-catalog/ | [spaceshied-catalog](https://github.com/heyjyu/spaceshied-catalog) |

## 도구 추가 방법

`index.html`의 `TOOLS` 배열에 항목 하나만 추가하면 카드가 자동 생성된다.

```js
{ num: '04', ico: '🧾', name: '새 도구', desc: '설명', url: 'https://…', repo: 'repo-name' }
```

정적 페이지(순수 HTML/CSS/JS, 빌드 없음) — 커밋 & 푸시하면 GitHub Pages에 바로 반영.

관련 이슈: [#1 통합 '회사 관리' 허브로 묶기](https://github.com/heyjyu/spaceshied-hub/issues/1)
