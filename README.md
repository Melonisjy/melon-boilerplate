# Melon Boilerplate

Next.js, TypeScript, Zustand, TanStack Query를 사용한 프론트엔드 보일러플레이트입니다.

## 기술 스택

- **Next.js 14** (App Router)
- **TypeScript**
- **Zustand** (상태 관리)
- **TanStack Query** (데이터 페칭)
- **Tailwind CSS** (스타일링)

## 프로젝트 구조

```
src/
├─ app/                    # Next.js App Router
│  ├─ layout.tsx          # 루트 레이아웃
│  ├─ page.tsx            # 홈 페이지
│  ├─ providers.tsx       # TanStack Query Provider
│  ├─ globals.css         # 전역 스타일
│  └─ (routes)/           # 라우트 그룹
│     ├─ home/
│     └─ profile/
│
├─ features/              # 기능별 모듈
│  ├─ auth/              # 인증 기능
│  │  ├─ api/           # API 호출
│  │  ├─ hooks/         # 커스텀 훅
│  │  ├─ store/         # Zustand 스토어
│  │  ├─ ui/            # UI 컴포넌트
│  │  └─ types.ts       # 타입 정의
│  └─ post/             # 게시글 기능
│
├─ shared/               # 공유 모듈
│  ├─ api/              # API 클라이언트
│  ├─ ui/               # 공통 UI 컴포넌트
│  ├─ lib/              # 유틸리티 함수
│  └─ types/            # 공통 타입
│
├─ stores/               # 전역 스토어
└─ styles/              # 스타일 파일
```

## 시작하기

### 설치

```bash
npm install
```

### 개발 서버 실행

```bash
npm run dev
```

브라우저에서 [http://localhost:3000](http://localhost:3000)을 열어 확인하세요.

### 빌드

```bash
npm run build
```

### 프로덕션 실행

```bash
npm start
```

## 환경 변수

`.env.local` 파일을 생성하고 다음 변수를 설정하세요:

```env
NEXT_PUBLIC_API_URL=http://localhost:3000/api
```
