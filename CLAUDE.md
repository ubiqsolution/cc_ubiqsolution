# 프로젝트: ubiqsolution 랜딩페이지

## GitHub
- https://github.com/ubiqsolution/cc_ubiqsolution
- 브랜치: main
- 도메인: https://ubiqsolution.pages.dev
- 사이트맵: https://ubiqsolution.pages.dev/sitemap.xml

## 프로젝트 구조
- index.html — 메인 랜딩페이지 (핵심 파일)
- privacy.html — 개인정보처리방침 (Editorial 디자인 적용)
- terms.html — 이용약관 (Editorial 디자인 적용)
- styles.css — 메인 디자인 시스템 (토큰, Header/Hero/섹션/CTA/Footer)
- legal.css — 법적 페이지 전용 스타일 (TOC, article, table, back 버튼)
- favicon.png — 파비콘 (U 심볼 아이콘, 블루 계열)
- ogimg.png — OG 이미지 (다크 배경 + UBIQ SOLUTION + AI & IT Company)
- logo.png — 구버전 로고 이미지 (현재 미사용, 텍스트 마크로 대체됨)
- sitemap.xml — 사이트맵 (3개 페이지 등록)
- robots.txt — 크롤링 규칙
- naver8bdb95fe081d2ea8ecae0db3fb612b5b.html — 네이버 서치어드바이저 인증
- _headers — Cloudflare Pages 보안 헤더 (CSP, X-Frame-Options 등)
- AGENTS.md — AI 에이전트 규칙
- .gitignore — git 제외 설정 (.env, *.log, node_modules/ 등)

## 기술 스택
- HTML5 + 커스텀 CSS (Tailwind 미사용)
- Pretendard (jsdelivr CDN)
- Vanilla JavaScript (FAQ 토글, IntersectionObserver reveal, 스크롤탑, smooth scroll)

## 디자인 시스템 (Editorial / Swiss Modern)
- **컬러**:
  - `--ink: #0E0E0C` (잉크)
  - `--paper: #F2EDE5` (크림)
  - `--paper-2: #E8E1D5`
  - `--accent: #D4F542` (라임)
- **폰트**: Pretendard (한글 우선)
- **타이포 강조**: `<em>` 태그로 italic 강조
- **반응형**: 4열/2열/1열 자동 재배치 (clamp 기반 fluid 사이즈)
- **로고**: `.logo-mark` (사각형+원 SVG) + `UBIQSOLUTION` 텍스트 (logo.png 미사용)

## 페이지 섹션 구성
**index.html**: Header → Hero(stamp 레이아웃) → Marquee(ink) → Why Us(4분할) → Marquee(paper) → Services(가로 행 리스트) → Target(6분할) → Process(4단계) → FAQ(아코디언) → CTA(다크 배경) → Footer

**privacy.html / terms.html**: Header → Legal Meta → 거대 H1 → Lead → TOC(2열) → Article(좌측 번호 + 우측 본문) ×N → Back 버튼 → Footer

## 핵심 서비스
- AI 컨설팅
- AI Agent 개발
- 데이터 분석 플랫폼

## 사업자 정보 (Footer)
- 상호: 유비큐솔루션
- 대표: 김시기
- 사업자등록번호: 132-10-98552
- 주소: 경기도 구리시 아차산로500번길 16 102호
- 전화: 1600-5693
- 이메일: 9292@ubiqsolution.com
- 상담시간: 평일 AM 10:00 ~ PM 17:00

## SEO / AEO 적용 현황
- meta description, canonical URL (3개 페이지 모두)
- meta keywords (AI컨설팅, 랜딩페이지, 유비큐솔루션, 시드팜 등)
- meta robots (index, follow)
- Open Graph (og:title, og:description, og:image, og:url, og:site_name)
- OG/Twitter 이미지 캐시 버스팅 적용 (`ogimg.png?v=2`)
- Twitter Card (summary_large_image + twitter:image)
- JSON-LD 구조화 데이터 (Service + keywords, FAQPage)
- JSON-LD 회사 주소 (경기도 구리시 아차산로500번길 16 102호)
- robots.txt, sitemap.xml
- favicon, og:image
- 네이버 서치어드바이저 인증

## UI 기능
- 스크롤 탑 버튼 — 전체 페이지 (스크롤 600px 이상 시 우측 하단)
- FAQ 아코디언 — 한 개만 열림, 키보드(Enter/Space) 접근 가능
- IntersectionObserver 기반 reveal-on-scroll (`.reveal` 클래스)
- 마키 텍스트 흐름 (38초 무한 루프, ink/paper 2개 변형)
- Smooth scroll (in-page 앵커)
- Hero 배경 동영상 — **제거됨** (정적 디자인으로 변경)

## 보안
- Cloudflare 보안 헤더 (_headers 파일)
  - CSP: 'self' + Pretendard CDN(jsdelivr) + Google Fonts만 허용 (Tailwind CDN 제거됨)
  - X-Frame-Options: DENY (클릭재킹 차단)
  - X-Content-Type-Options: nosniff
  - Referrer-Policy: strict-origin-when-cross-origin
  - Permissions-Policy: 카메라/마이크/위치 차단
- .gitignore: .env, *.log, node_modules/, IDE 설정 등 제외

## 세션 시작 루틴
1. `git log --oneline -10` 실행해서 최근 작업 확인
2. `git status` 로 현재 변경사항 확인
3. index.html / styles.css 구조 파악
4. 이 파일 규칙 숙지 후 현황 요약

## 보호 규칙
- 완성된 섹션은 수정 금지
- 새 섹션/기능만 추가
- 수정 필요시 반드시 먼저 확인 요청
- 커밋 전 git diff 확인
- SEO 메타/JSON-LD는 임의 변경 금지 (description 보강 등은 사전 확인)

## 작업 후 커밋 루틴
1. `git add .` 또는 명시적 파일 지정
2. `git commit -m "작업내용 간단 설명"`
3. `git push origin main` (사용자 확인 후)

---

## 이후 매 세션 시작 프롬프트 (한 줄)
```
CLAUDE.md 읽고 프로젝트 현황 파악해줘
```
