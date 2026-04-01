# 윤제훈 비즈니스 프로필 홈페이지

## 프로젝트 개요
연쇄 창업가 윤제훈의 비즈니스 프로필 홈페이지입니다.  
다크 테마 + 시그니처 오렌지 포인트 컬러로 강렬하고 모던한 인상을 전달하며, 실행력과 비즈니스 성과를 직관적으로 보여줍니다.

---

## ✅ 구현된 기능

### 디자인
- 다크 테마 (`#111111` 배경) + 시그니처 오렌지(`#FF5A36`) 포인트 컬러
- Glassmorphism 카드 효과 (backdrop-filter blur)
- 카드 호버 시 `translateY(-6px)` + 오렌지 글로우 `box-shadow` 애니메이션
- Pretendard 폰트 적용 및 최적화 (Preconnect/Preload)
- 인터랙티브 캔버스 파티클 배경 (모바일/PC 반응형 성능 최적화)

### 네비게이션 & UX
- 스크롤 시 고정(sticky) 네비게이션 바 및 배경 블러 효과
- Intersection Observer 기반 활성 섹션 하이라이트
- GPU 가속(`transform: scaleX`)을 활용한 최적화된 스크롤 진행 바(Progress bar)
- 클립보드 복사 헬퍼 기능 (이메일, 프로필 URL)

### 애니메이션
- Intersection Observer를 활용한 스크롤 `fade-in-up` 등장 애니메이션
- 프로필 헤더 뱃지 pulse/spin 글로우 효과
- 자연스러운 감속(ease-out)이 적용된 숫자 카운트업 효과 (매출 11억+)
- CSS keyframes를 활용한 부드러운 스크롤 유도 화살표 바운스

### 콘텐츠 섹션
- **Hero 헤더**: 뱃지, 타이틀, 프로필 사진, 소개 텍스트, CTA 버튼
- **Stats 수치**: 4개 주요 지표 카드 그리드
- **Experience**: 6개 경력 카드 (대형 4개 + 소형 2개 + 공군)
- **Highlights**: 4개 주요 수상/성과
- **Education**: 학력 + Military 섹션 (공군 복무)
- **Contact Footer**: 전화/이메일/인스타그램/URL복사 연결 버튼

### 반응형
- 모바일 / 태블릿 / 데스크톱 완전 대응
- Tailwind CSS 유틸리티 + 커스텀 CSS 조합

---

## 📁 파일 구조

```
index.html          # 메인 HTML (CSS, JS 통합 단일 파일 구조)
images/
  profile.jpg       # 프로필 사진
README.md
```

---

## 🔗 주요 경로

| 경로 | 설명 |
|------|------|
| `/` | 메인 프로필 페이지 |
| `/#stats` | 핵심 수치 섹션 |
| `/#strengths` | 핵심 역량 섹션 |
| `/#experience` | 경력 섹션 |
| `/#highlights` | 수상/성과 + 학력/병역 섹션 |
| `/#contact` | 연락처 섹션 |

---

## ⚠️ 추후 개선 사항

- [ ] OG 이미지 교체 (SNS 공유 미리보기용)
- [ ] 다국어 지원 (영문 버전)
- [ ] 다운로드 가능한 PDF 이력서 연동
- [ ] 포트폴리오 상세 페이지 (프로젝트별)

---

## 🛠 사용 기술

- **HTML5 / CSS3 / Vanilla JS** (순수 프론트엔드)
- **Tailwind CSS** (CDN) — 유틸리티 스타일링
- **Pretendard** 폰트 (CDN)
- **Intersection Observer API** — 스크롤 및 카운트업 애니메이션
- **requestAnimationFrame** — 카운트업 프레임 렌더링
- **HTML5 Canvas** — 배경 파티클 효과

---

*© 2026 Jehoon Yun. All rights reserved.*
