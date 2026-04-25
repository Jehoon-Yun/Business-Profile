# 윤제훈 비즈니스 프로필 홈페이지

## 프로젝트 개요
연쇄 창업가 윤제훈의 비즈니스 프로필 홈페이지입니다.
다크 테마 + 시그니처 오렌지 포인트 컬러로 강렬하고 모던한 인상을 전달하며, 실행력과 비즈니스 성과를 직관적으로 보여줍니다.

🔗 **Live**: <https://jehoon-yun.github.io/Business-Profile/>

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
- 클립보드 복사 기능 (이메일, 프로필 URL) — `addEventListener` 기반

### 애니메이션
- Intersection Observer를 활용한 스크롤 `fade-in-up` 등장 애니메이션
- 프로필 헤더 뱃지 pulse/spin 글로우 효과
- 자연스러운 감속(ease-out)이 적용된 숫자 카운트업 효과 (매출 11억+)
- CSS keyframes를 활용한 부드러운 스크롤 유도 화살표 바운스

### 접근성 (a11y)
- `prefers-reduced-motion` 미디어쿼리 지원 — 동작 줄이기 사용자에게 모든 애니메이션/파티클/카운트업 자동 비활성화
- `focus-visible` 키보드 포커스 인디케이터 (시그니처 오렌지)
- 배경 캔버스 `aria-hidden="true"` 처리
- h1에 검색엔진/스크린리더 전용 이름 숨김 텍스트(`sr-only`)

### SEO & 메타데이터
- JSON-LD Schema.org `Person` 타입 — `founder`(4개 회사), `worksFor`, `memberOf` 관계 명시
- Open Graph + Twitter Card 메타 태그
- canonical URL, sitemap.xml, robots.txt 완비
- 구글 사이트 검증(google-site-verification) 메타 적용

### 콘텐츠 섹션
- **Hero 헤더**: 뱃지, 타이틀, 프로필 사진, 소개 텍스트, CTA 버튼
- **Stats 수치**: 4개 주요 지표 카드 그리드
- **Experience**: 6개 경력 카드 (대형 4개 + 소형 2개)
- **Highlights**: 5개 주요 수상/성과
- **Education**: 학력 + Military 섹션 (공군 복무)
- **Contact Footer**: 카카오톡/이메일/URL복사/인스타그램 연결 버튼

### 반응형
- 모바일 / 태블릿 / 데스크톱 완전 대응
- Tailwind CSS 유틸리티 + 커스텀 CSS 조합

---

## 📁 파일 구조

```
index.html              # 메인 HTML (CSS, JS 통합 단일 파일 구조)
output.css              # 사전 컴파일된 Tailwind CSS
sitemap.xml             # 검색엔진용 사이트맵
robots.txt              # 크롤러 제어
site.webmanifest        # PWA 매니페스트
images/
  profile.jpg           # 프로필 사진
  konkuk-logo.webp      # 건국대학교 로고
  favicon.ico
  favicon-16x16.png
  favicon-32x32.png
  apple-touch-icon.png
  android-chrome-192x192.png
  android-chrome-512x512.png
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

## 🔧 최근 개선 사항 (2026.04)

### SEO 강화
- h1 태그에 `sr-only` 기법으로 본인 이름 키워드 추가 (시각 디자인은 그대로)
- JSON-LD에 `founder` (유니브립·림픽컴퍼니·산호초메디컬·에셋코치), `worksFor` (디렉터홀딩스), `memberOf` (대한민국 공군) 관계 추가 — 구글이 인물-조직 관계를 정확히 이해

### 접근성 보강
- `prefers-reduced-motion` 미디어쿼리 지원 — 멀미·전정 장애 사용자 보호
- 키보드 사용자를 위한 `focus-visible` 오렌지 인디케이터
- 배경 파티클 캔버스에 `aria-hidden` 추가 (스크린리더 무시)

### 개인정보 보호
- 휴대폰 번호 노출 제거 (페이지·JSON-LD 모두) — 스미싱·스팸 위험 차단
- 1차 컨택 채널을 카카오톡 오픈프로필로 변경

### 코드 품질
- 모든 인라인 `style="..."` 속성을 CSS 클래스로 분리 (총 11곳)
- 인라인 `onclick="..."` 핸들러를 `addEventListener` 방식으로 전환 (CSP 호환성 ↑)
- 사용되지 않는 죽은 코드(`<p id="url-display">`) 제거

---

## ⚠️ 추후 개선 사항

- [ ] OG 이미지 교체 (1200×630 전용 카드 디자인 — SNS 공유 미리보기용)
- [ ] 다국어 지원 (영문 버전)
- [ ] 다운로드 가능한 PDF 이력서 연동
- [ ] 포트폴리오 상세 페이지 (프로젝트별 케이스 스터디)
- [ ] 모바일 햄버거 네비게이션 추가
- [ ] 경력 카드별 본인 기여도/임팩트 명시 보강

---

## 🛠 사용 기술

- **HTML5 / CSS3 / Vanilla JS** (순수 프론트엔드)
- **Tailwind CSS** — 사전 컴파일된 `output.css`로 정적 제공
- **Pretendard** 폰트 (CDN — `pretendard-dynamic-subset.min.css`)
- **Intersection Observer API** — 스크롤 등장·카운트업·네비게이션 활성화
- **requestAnimationFrame** — 카운트업 프레임 렌더링
- **HTML5 Canvas** — 배경 파티클 효과
- **Schema.org JSON-LD** — 구조화된 데이터로 검색엔진 최적화

---

## 🚀 배포

GitHub Pages로 정적 호스팅. `main` 브랜치에 푸시하면 자동 배포됩니다.

배포 후 검증 도구:
- [Google Rich Results Test](https://search.google.com/test/rich-results) — JSON-LD 인식 확인
- [Schema Markup Validator](https://validator.schema.org/) — 스키마 유효성 검증
- [PageSpeed Insights](https://pagespeed.web.dev/) — 성능·접근성 점수

---

*© 2026 Jehoon Yun. All rights reserved.*
