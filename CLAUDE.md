# dev-hub 작업 규칙

## "오늘 작업 기록해줘" 명령 시 워크플로우

1. Notion 작업일지 검색/업데이트
2. Notion 진척도 업데이트
3. 로컬 파일 수정 (file:/// 절대 경로 유지):
   - C:\Vs\dev-hub.html
   - C:\Vs\results.html
4. GitHub용 파일 수정 (상대 경로 유지):
   - C:\Vs\dev-hub\dev-hub.html
   - C:\Vs\dev-hub\results.html
5. git push → C:\Vs\dev-hub\ (galincia-hub/dev-hub)

## 경로 규칙

- 로컬용: `file:///C:/Vs/...` 형식
- GitHub용: `mockups/...`, `_site/...` 등 상대 경로 (mockups 섹션만)

## 주요 경로 매핑

| 항목 | 경로 |
|------|------|
| 상품카드 | `CruiseMD/products/product_cards_v2_latest.html` |
| sailings | `CruiseMD/data/sailings_index.json` |
| 목업 홈 | `cruise-site/_site/index.html` |
| 목업 선사 | `cruise-site/_site/regent/index.html` |
| 목업 상품 | `cruise-site/_site/regent/med-splendor-2026-06/index.html` |
| 목업 블로그 | `cruise-site/_site/blog/index.html` |
| blog_V2 | `blog_V2/.mcp.json` (CLAUDE.md 없음) |

## 사이트 미리보기

```bash
cd C:/Vs/cruise-site/_site && python -m http.server 4000
# http://localhost:4000
```

## 저장소 구조

| 역할 | 로컬 경로 | GitHub |
|------|-----------|--------|
| Jekyll 사이트 | C:\Vs\cruise-site\ | galincia-hub/cruise-website |
| dev-hub (GitHub용) | C:\Vs\dev-hub\ | galincia-hub/dev-hub |
| dev-hub (로컬 전용) | C:\Vs\dev-hub.html | — |
| results (로컬 전용) | C:\Vs\results.html | — |
