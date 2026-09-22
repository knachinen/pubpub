---
id: "2025-1212_5-346-50_110718"
date: "2025-12-12"
time: "2025-12-12T11:07:18"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] 포트폴리오 웹페이지
> - 인터랙티브 포트폴리오 웹페이지

---

## 개발환경

> [!INFO] IDE & 모델
> - Gemini 2.5 Fast / Claude Sonnet 4.5 / ChatGPT / Grok Auto
> 	- 기획안 및 제품 요구사항 명세서 작성
> - Google Stitch
> 	- 목업 디자인
> - Gemini CLI
> 	- 계획, 구현, 디버깅: Gemini 2.5 Auto, Flash


---

## 작업 요청

### 기획안 및 제품 요구사항 명세서 작성 
Gemini Fast, Claude Sonnet 4.5, ChatGPT, Grok Auto

> [!QUESTION] 프롬프트
> - 1인 창업자 대상 인터랙티브 브랜드 포트폴리오 웹사이트 기획안 작성
> - 제품 요구사항 명세서 작성
> - 현재 버전을 모두 잊을 것. 기술스택 하나씩 다시 검색해서 최신버전을 찾기. 참고한 문서 링크 첨부
> - 단계별 구현 계획 작성. 단계별로 독립적인 실행이 가능해야 함. 
> - 1단계 구현 상세 계획
> - 2단계 구현 상세 계획
> - 3단계 구현 상세 계획
> - 4단계 구현 상세 계획
> - 5단계 구현 상세 계획


> [!EXAMPLE] 기획안 및 제품 요구사항 명세서
> - [Gemini](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/plan_gemini.md)
> - [Claude](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/plan_claude.md)
> - [ChatGPT](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/plan_chatgpt.md)
> - [Grok](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/plan_grok.md)


> [!EXAMPLE] 단계별 구현계획
> - [단계별 구현계획](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/plan_phase.md)
> - [1단계 구현계획](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/plan_phase-1.md)
> - [2단계 구현계획](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/plan_phase-2.md)
> - [3단계 구현계획](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/plan_phase-3.md)
> - [4단계 구현계획](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/plan_phase-4.md)
> - [5단계 구현계획](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/plan_phase-5.md)


### 목업 디자인 
Stitch, Gemini

![[p18-w03-5_mockup.png]]

> [!QUESTION] Stitch 목업 디자인
> - 기획안과 제품 요구사항 명세서를 바탕으로 웹디자인
> 	- (기획안 및 제품 요구사항 명세서 내용 첨부)

> [!QUESTION] Gemini 디자인 명세서 작성
> - 000 섹션 디자인 명세서 작성. 
> - 색상 코드와 폰트 정보 명세서 작성. 
> - 간격 및 정렬, 인터랙션 및 애니메이션, 접근성 및 SEO 명세서 작성.
> - (컬러 팔레트, 간격 및 정렬, 인터랙션 및 애니메이션, 접근성 및 SEO, 폰트 명세서 작성)


> [!EXAMPLE] 디자인 명세서
> - [섹션 1 - 히어로](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/design_section-1.md)
> - [섹션 2 - 소개](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/design_section-2.md)
> - [섹션 3 - 포트폴리오](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/design_section-3.md)
> - [섹션 4 - 서비스](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/design_section-4.md)
> - [섹션 5 - 후기](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/design_section-5.md)
> - [섹션 6 - 연락처](https://github.com/knachinen/one-day-one-project/blob/main/p18-w03-5_portfolio/doc/design_section-6.md)


### 작업 요청 
Gemini CLI

> [!QUESTION] 구현 프롬프트
> - 1단계 구현
> - 섹션 1 구현
> - 섹션 2 구현
> - 섹션 3 구현
> - 섹션 4 구현
> - 섹션 5 구현
> - 섹션 6 구현
> - 2단계 구현
> - 3단계 구현
> - 4단계 구현


---

## 개발 과정 

### 구현 후 첫 실행

단계별로 구현 및 실행 검증을 함. 

### 구현 기능 검증

> [!BUG] 
> - `use Client;` 매 섹션마다 빠뜨림.
> - `via.placeholder.com` 
> - `shadcn/ui`
> - `<motion.div unoptimized></motion.div>`

### 수정 보완

> [!BUG] 
> - Header, Footer 메인 테마 적용
> - 단어 띄어쓰기



---
## 결과 

![[p18-w03-5_screen.png]]

### 미완성

> [!BUG] 
> - 비디오 플레이스홀더 
> - 프로젝트 프로세스 수직 라인 
> - '프로젝트 시작하기' 버튼 액션
> - 사진 첨부 및 SNS 링크 


### 완료

> [!SUCCESS] 
> - 대부분의 구현 계획
> - 목업 디자인 적용



---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p18_w03-5_portfolio](https://github.com/knachinen/one-day-one-project/tree/main/p18-w03-5_portfolio) (github.com)
