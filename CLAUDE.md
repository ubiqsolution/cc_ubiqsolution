# 프로젝트: ubiqsolution 랜딩페이지

## GitHub
- https://github.com/ubiqsolution/cc_ubiqsolution
- 브랜치: main
- 도메인: https://ubiqsolution.pages.dev

## 프로젝트 구조
- index.html — 메인 랜딩페이지 (핵심 파일)
- privacy.html — 개인정보처리방침
- terms.html — 이용약관
- logo.png — 로고 이미지 (32x32 표시, Header/Footer 사용)
- favicon.png — 파비콘
- ogimg.png — OG 이미지 (소셜 공유용)
- sitemap.xml — 사이트맵
- robots.txt — 크롤링 규칙
- AGENTS.md — AI 에이전트 규칙
- .gitignore — git 제외 설정

## 기술 스택
- HTML / Tailwind CSS (CDN)
- Google Fonts (Noto Sans KR)

## SEO / AEO 적용 현황
- meta description, canonical URL
- Open Graph (og:title, og:description, og:image, og:url)
- Twitter Card (summary_large_image)
- JSON-LD 구조화 데이터 (Service, FAQPage)
- robots.txt, sitemap.xml
- favicon, og:image

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
