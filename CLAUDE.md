# 생각 (휴대폰 생각 넣기·오늘 보기)

대표 휴대폰 홈 화면에 설치하는 웹 앱(PWA). 한 줄을 넣으면 업무 보드 인풋 > 생각에 들어가고, 아래에서 오늘 일정·오늘 할 일·위임 · 오늘 마감을 본다(보기만).

| 항목 | 내용 |
|---|---|
| 계획서·화면안 | 업무 보드 저장소 `paranbanbazi/paek4.0`의 `자료/휴대폰 생각 넣기 계획서.md`, `자료/휴대폰 생각 넣기 화면안.html`(PNG) 3판 |
| 주소 | https://paranbanbazi.github.io/thought-inbox/ (GitHub Pages, main 브랜치 루트) |
| 서버 | Supabase Edge Function `thought-inbox`(코드는 업무 보드 저장소 `supabase/functions/thought-inbox`) |
| 비밀 값 | 함수 비밀 `THOUGHT_INBOX_KEY`(Supabase 대시보드 / Edge Functions Secrets). 휴대폰에는 연결 QR(`tools/thought-inbox/new-key.mjs`, 업무 보드 저장소)로만 들어간다 |
| 파일 | `index.html`(화면·동작 전부), `manifest.webmanifest`, 아이콘 |

## 규칙

- 이 저장소는 **공개**다. 비밀 값·서비스 키·공개 키·고객 이름을 파일·커밋·이슈에 넣지 않는다. 함수 주소만 둔다.
- 넣기만 한다. 사업체·거래처·기한·명료화·처리 고르기, 할 일 체크·고치기는 넣지 않는다(처리는 PC 보드).
- 오늘 목록은 휴대폰에 저장하지 않는다(쓰던 글·연결 값만 저장).
- 빌드 없음. 고치면 main에 올리고 1~2분 뒤 휴대폰에서 다시 열면 바뀐다.
- 확인: 휴대폰 폭(390)으로 화면안 4~8 상태와 대조.
