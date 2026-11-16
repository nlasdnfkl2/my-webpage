# 오운완! 운동 기록 저장 · 월간 통계 PWA (실습 18)

GitHub Pages에 업로드하면 스마트폰 홈 화면에 설치하여 오프라인에서도 일반 모바일 앱처럼 사용할 수 있는 PWA(Progressive Web App) 패키지입니다.

## 포함된 파일 구성
1. `phycheck.html` — 메인 앱 화면 (`index.html` 포트폴리오와 바로 연결되는 파일명)
2. `manifest.json` — 앱 이름, 아이콘, 독립 실행(`standalone`) 화면 설정 파일
3. `sw.js` — 오프라인 캐시 및 앱 설치 조건을 충족하는 서비스 워커(Service Worker)
4. `icon-192.png` — 모바일 홈 화면 아이콘 (192x192)
5. `icon-512.png` — 모바일 스플래시 및 고해상도 아이콘 (512x512)

## GitHub 업로드 및 모바일 앱 설치 순서
1. 위 5개 파일(`phycheck.html`, `manifest.json`, `sw.js`, `icon-192.png`, `icon-512.png`)을 모두 **같은 폴더(리포지토리 루트)**에 업로드합니다.
   - *(참고: 별도의 단독 리포지토리로 만들 경우 `phycheck.html`을 `index.html`로 복사하고 `manifest.json`과 `sw.js`의 `phycheck.html` 경로를 `index.html`로 맞추면 루트 URL로 바로 열립니다.)*
2. GitHub 리포지토리의 **Settings → Pages → Branch (`main` / `/root`)**를 활성화합니다.
3. 스마트폰 브라우저로 배포된 주소(`https://nlasdnfkl2.github.io/리포지토리명/phycheck.html`)에 접속합니다.
   - **Android (Chrome):** 상단 **[+ 지금 앱 설치]** 버튼 또는 우측 상단 **[⋮] → [앱 설치]** 터치
   - **iPhone (Safari):** 하단 **[공유(□↑)] → [홈 화면에 추가]** 터치
