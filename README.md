# NVDA 주가 맥락 탐색기

## 빠른 시작

### 1. Node.js 설치
- https://nodejs.org 에서 LTS 버전 다운로드 (v18 이상)

### 2. 의존성 설치
```bash
cd nvda-app
npm install
```

### 3. 개발 서버 실행
```bash
npm run dev
```

### 4. 브라우저에서 열기
터미널에 표시되는 URL (보통 http://localhost:5173) 접속

---

## 프로덕션 빌드

```bash
npm run build
npm run preview
```

`dist/` 폴더가 생성되며, 이를 Vercel / Netlify / GitHub Pages 등에 배포할 수 있습니다.

## Vercel 배포 (가장 간단)

1. https://vercel.com 에서 GitHub 연동
2. 이 폴더를 GitHub repo에 push
3. Vercel에서 import → 자동 빌드 & 배포
4. URL 발급됨 (예: nvda-viewer.vercel.app)

## 구조

```
nvda-app/
├── index.html          # HTML 엔트리
├── package.json        # 의존성
├── vite.config.js      # Vite 설정
├── src/
│   ├── main.jsx        # React 엔트리
│   └── App.jsx         # 메인 컴포넌트 (차트 + 내러티브 + 이벤트)
└── README.md
```
