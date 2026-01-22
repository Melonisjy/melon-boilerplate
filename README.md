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
│  ├─ layout.tsx           # 루트 레이아웃
│  ├─ page.tsx             # 홈 페이지
│  ├─ providers.tsx        # TanStack Query Provider
│  ├─ globals.css          # 전역 스타일
│  └─ (routes)/            # 라우트 그룹
│     ├─ home/
│     └─ profile/
│
├─ features/               # 기능별 모듈
│  ├─ auth/                # 인증 기능
│  │  ├─ api/              # API 호출
│  │  ├─ hooks/            # 커스텀 훅
│  │  ├─ store/            # Zustand 스토어
│  │  ├─ ui/               # UI 컴포넌트
│  │  └─ types.ts          # 타입 정의
│  └─ post/                # 게시글 기능
│
├─ shared/                 # 공유 모듈
│  ├─ api/                 # API 클라이언트
│  ├─ ui/                  # 공통 UI 컴포넌트
│  ├─ lib/                 # 유틸리티 함수
│  └─ types/               # 공통 타입
│
├─ stores/                 # 전역 스토어
└─ styles/                 # 스타일 파일
```
