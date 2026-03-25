# 프로젝트: ubiqsolution 랜딩페이지

## GitHub
- https://github.com/ubiqsolution/cc_ubiqsolution
- 브랜치: main
- 도메인: https://ubiqsolution.pages.dev
- 사이트맵: https://ubiqsolution.pages.dev/sitemap.xml

## 프로젝트 구조
- index.html — 메인 랜딩페이지 (핵심 파일)
- privacy.html — 개인정보처리방침
- terms.html — 이용약관
- logo.png — 로고 이미지 (UBIQ SOLUTION 흰색 텍스트, 투명배경, Header/Footer 사용)
- favicon.png — 파비콘 (U 심볼 아이콘, 블루 계열)
- ogimg.png — OG 이미지 (다크 배경 + UBIQ SOLUTION + AI & IT Company)
- sitemap.xml — 사이트맵 (3개 페이지 등록)
- robots.txt — 크롤링 규칙
- naver8bdb95fe081d2ea8ecae0db3fb612b5b.html — 네이버 서치어드바이저 인증
- _headers — Cloudflare Pages 보안 헤더 (CSP, X-Frame-Options 등)
- AGENTS.md — AI 에이전트 규칙
- .gitignore — git 제외 설정 (.env, *.log, node_modules/ 등)

## 기술 스택
- HTML / Tailwind CSS (CDN)
- Google Fonts (Noto Sans KR)

## 로고 사이즈
- Header: PC 220px / 모바일 170px (h-auto)
- Footer: PC 200px / 모바일 160px (h-auto)
- privacy, terms 페이지: PC 180px / 모바일 140px (h-auto)
- 로고 옆 텍스트 없음 (이미지만 사용)

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

## SEO / AEO 적용 현황
- meta description, canonical URL
- meta keywords (AI컨설팅, 랜딩페이지, 유비큐솔루션, 시드팜 등)
- meta robots (index, follow)
- Open Graph (og:title, og:description, og:image, og:url)
- OG/Twitter 이미지 캐시 버스팅 적용 (`ogimg.png?v=2`)
- Twitter Card (summary_large_image + twitter:image)
- JSON-LD 구조화 데이터 (Service + keywords, FAQPage)
- JSON-LD 회사 주소 (경기도 구리시 아차산로500번길 16 102호)
- robots.txt, sitemap.xml
- favicon, og:image
- 네이버 서치어드바이저 인증

## UI 기능
- 스크롤 탑 버튼 — 전체 페이지 적용 (스크롤 400px 이상 시 우측 하단 표시)
- Hero 배경 동영상 오버레이 밝기 조정 (55%/45%)

## 보안
- Cloudflare 보안 헤더 (_headers 파일)
  - CSP: Tailwind CDN, Google Fonts만 허용
  - X-Frame-Options: DENY (클릭재킹 차단)
  - X-Content-Type-Options: nosniff
  - Referrer-Policy: strict-origin-when-cross-origin
  - Permissions-Policy: 카메라/마이크/위치 차단
- .gitignore: .env, *.log, node_modules/, IDE 설정 등 제외

## 세션 시작 루틴
1. `git log --oneline -10` 실행해서 최근 작업 확인
2. `git status` 로 현재 변경사항 확인
3. index.html 구조 파악
4. 이 파일 규칙 숙지 후 현황 요약

## 보호 규칙
- 완성된 섹션은 수정 금지
- 새 섹션/기능만 추가
- 수정 필요시 반드시 먼저 확인 요청
- 커밋 전 git diff 확인

## 작업 후 커밋 루틴
1. `git add .`
2. `git commit -m "작업내용 간단 설명"`
3. `git push origin main`

---

## 이후 매 세션 시작 프롬프트 (한 줄)
```
CLAUDE.md 읽고 프로젝트 현황 파악해줘
```
