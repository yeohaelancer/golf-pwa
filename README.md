# ⛳ 골프 스코어 PWA

별도 앱 설치 없이 브라우저에서 바로 사용하는 골프 스코어 기록 앱입니다.

---

## 배포 방법 (무료)

### 방법 1: GitHub Pages (추천)

1. [github.com](https://github.com) 무료 계정 생성
2. 새 Repository 만들기 (이름 예: `golf-score`)
3. 이 폴더의 파일을 모두 업로드
4. Settings → Pages → Branch: main → Save
5. 몇 분 후 `https://[계정명].github.io/golf-score` 로 접속 가능

### 방법 2: Netlify (가장 쉬움)

1. [netlify.com](https://netlify.com) 접속
2. 로그인 없이 이 폴더를 통째로 드래그 & 드롭
3. 즉시 URL 발급 (예: `https://random-name.netlify.app`)

---

## 폰 홈화면에 추가하는 방법

### Android (Chrome)
1. 위 URL을 Chrome으로 열기
2. 주소창 오른쪽 메뉴(⋮) → "홈 화면에 추가"
3. 이름 확인 후 "추가" 탭

### iPhone (Safari)
1. Safari로 URL 열기 (**반드시 Safari 사용**)
2. 하단 공유 버튼(□↑) 탭
3. "홈 화면에 추가" 탭
4. 이름 확인 후 "추가" 탭

---

## 파일 구조

```
golf-pwa/
├── index.html          ← 앱 전체 (단일 파일)
├── manifest.json       ← PWA 설정
├── sw.js               ← 오프라인 지원
└── icons/
    ├── icon-192.png
    ├── icon-512.png
    └── apple-touch-icon.png
```

---

## 특징

- 설치 없이 브라우저에서 바로 실행
- Android / iPhone 모두 지원
- 오프라인에서도 동작 (Service Worker)
- 데이터는 기기 로컬에 저장 (localStorage)
- 홈화면 추가 시 앱처럼 전체화면으로 실행
