# commute-navi

출발지에서 도착지까지 **TMAP · 카카오맵 · 네이버지도** 세 가지 길안내를 한 화면에서 비교하고,
가장 빠른 길로 바로 안내를 시작하는 단일 HTML 앱입니다.

- https://keunchui.github.io/commute-navi/ — GitHub Pages로 배포됩니다.
- GPS는 HTTPS(보안 연결)에서만 동작합니다.
- 도착지·테스트 출발지·API 키는 브라우저(localStorage)에만 저장되며 서버로 전송되지 않습니다.
  이 저장소에는 개인 주소나 좌표가 들어 있지 않습니다.

## 링크로 설정 넘기기 (선택)

아래 파라미터를 URL 해시로 붙이면 열 때 한 번 읽어 브라우저에 저장하고 주소창에서 해시를 지웁니다.
해시는 서버로 전송되지 않습니다.

```
https://keunchui.github.io/commute-navi/#dname=도착지이름&daddr=도착지주소&dlat=35.1&dlng=129.0&tname=테스트출발지&taddr=주소&tlat=35.1&tlng=129.0
```

## 파일

- `index.html` — 앱 전체 (외부 의존성 없음)
- `.github/workflows/deploy.yml` — `main` 브랜치 푸시 시 Pages 배포
