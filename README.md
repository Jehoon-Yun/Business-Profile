# 윤제훈 비즈니스 프로필 홈페이지

## 프로젝트 개요
연쇄 창업가 윤제훈의 비즈니스 프로필 홈페이지입니다.  
다크 테마 + 라임 그린 포인트 컬러로 강렬하고 모던한 인상을 전달합니다.

---

## ✅ 구현된 기능

### 디자인
- 다크 테마 (`#111111` 배경) + 라임 그린(`#39FF14`) 포인트 컬러
- Glassmorphism 카드 효과 (backdrop-filter blur)
- 카드 호버 시 `translateY(-6px)` + 그린 `box-shadow` 애니메이션
- Pretendard 폰트 적용
- 미묘한 배경 방사형 그라데이션

### 네비게이션
- 스크롤 시 고정(sticky) 네비게이션 바
- 스크롤에 따라 배경 블러/반투명 효과
- 현재 섹션에 따른 활성 링크 하이라이트
- 모바일 햄버거 메뉴

### 애니메이션
- Intersection Observer를 활용한 스크롤 `fade-in-up` 등장 애니메이션
- 헤더 뱃지 pulse 글로우 효과
- 그린 그라데이션 텍스트 흐름 애니메이션
- 숫자 카운트업 효과 (총 누적 매출 11억+)
- 데스크톱 커서 포인트 효과 (mix-blend-mode)

### 콘텐츠 섹션
- **Hero 헤더**: 뱃지, 타이틀, 프로필 사진, 소개 텍스트, CTA 버튼
- **Stats 수치**: 4개 주요 지표 카드 그리드
- **Experience**: 6개 경력 카드 (대형 4개 + 소형 2개 + 공군)
- **Highlights**: 4개 주요 수상/성과
- **Education**: 학력 + Core Competencies 스킬 태그
- **Contact Footer**: 전화/이메일/인스타그램 연결 버튼

### 반응형
- 모바일 / 태블릿 / 데스크톱 완전 대응
- Tailwind CSS 유틸리티 + 커스텀 CSS 조합

---

## 📁 파일 구조

```
index.html          # 메인 HTML
css/
  style.css         # 커스텀 스타일 및 애니메이션
js/
  main.js           # 인터랙션 (Intersection Observer, 스크롤, 애니메이션)
README.md
```

---

## 🔗 주요 경로

| 경로 | 설명 |
|------|------|
| `/` | 메인 프로필 페이지 |
| `/#experience` | 경력 섹션 |
| `/#highlights` | 수상/성과 섹션 |
| `/#education` | 교육 섹션 |
| `/#contact` | 연락처 섹션 |

---

## ⚠️ 미구현 / 추후 개선 사항

- [ ] 실제 프로필 사진으로 교체 (현재 placeholder 이미지 사용 중)
- [ ] OG 이미지 실제 이미지로 교체
- [ ] 다국어 지원 (영문 버전)
- [ ] 다운로드 가능한 PDF 이력서 연동
- [ ] 포트폴리오 상세 페이지 (프로젝트별)
- [ ] 애니메이션 접근성 (`prefers-reduced-motion`) 대응

---

## 🛠 사용 기술

- **HTML5 / CSS3 / Vanilla JS** (순수 프론트엔드)
- **Tailwind CSS** (CDN) — 유틸리티 스타일링
- **Pretendard** 폰트 (CDN)
- **Intersection Observer API** — 스크롤 애니메이션
- **requestAnimationFrame** — 숫자 카운트업

---

*© 2026 Yun Je Hoon. All rights reserved.*
