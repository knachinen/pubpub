---
id: "2025-1215_1-349-51_100130"
date: "2025-12-15"
time: "2025-12-15T10:01:30"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] 제품 랜딩페이지
> - 제품 랜딩페이지

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

> [!QUESTION] 프롬프트: 기획안
> - 새로운 프로젝트: 제품 인터랙티브 랜딩페이지 기획안 작성
> - **제품 정보:**
> 	- 제품/서비스 종류: 바이브코딩 교육 워크숍
> 	- 타겟 고객층: 코딩 지식이 전혀없는 일반인
> 	- 핵심 가치 제안 (Value Proposition): 코딩 지식없이 MVP 완성
> 	- 경쟁사 대비 차별점: 3시간 오프라인 교육진행. 디버깅 후속 교육. 1인 창업자 맞춤교육.
> - **랜딩페이지 목표:**
> 	- 주요 전환 목표: 커뮤니티 가입
> 	- 원하는 브랜드 톤&매너: 친근함

> [!EXAMPLE] 기획안 및 제품 요구사항 명세서
> - [Gemini](https://github.com/knachinen/one-day-one-project/blob/main/p19-w04-1_landing/doc/plan_gemini.md)
> - [Claude](https://github.com/knachinen/one-day-one-project/blob/main/p19-w04-1_landing/doc/plan_claude.md)
> - [ChatGPT](https://github.com/knachinen/one-day-one-project/blob/main/p19-w04-1_landing/doc/plan_chatgpt.md)
> - [Grok](https://github.com/knachinen/one-day-one-project/blob/main/p19-w04-1_landing/doc/plan_grok.md)

> [!QUESTION] 프롬프트: 제품 요구사항 명세서, 기술 스택, 단계별 구현 계획
> - 제품 요구사항 명세서 작성
> - 단계별 구현 계획 작성. 단계별로 독립적인 실행이 가능해야 함. 

> [!QUESTION] 프롬프트: 단계별 구현 상세 계획
> - 제품 요구사항 명세서와 섹션별 디자인 상세 명세서를 바탕으로 phase-1 구현 계획 작성
> - 제품 요구사항 명세서와 섹션별 디자인 상세 명세서를 바탕으로 phase-2 구현 계획 작성
> - 제품 요구사항 명세서와 섹션별 디자인 상세 명세서를 바탕으로 phase-3 구현 계획 작성

> [!EXAMPLE] 단계별 구현계획
> - [단계별 구현계획](https://github.com/knachinen/one-day-one-project/blob/main/p19-w04-1_landing/doc/plan_implementation.md)
> 	- [1단계 구현계획](https://github.com/knachinen/one-day-one-project/blob/main/p19-w04-1_landing/doc/plan_phase-1.md)
> 	- [2단계 구현계획](https://github.com/knachinen/one-day-one-project/blob/main/p19-w04-1_landing/doc/plan_phase-2.md)
> 	- [3단계 구현계획](https://github.com/knachinen/one-day-one-project/blob/main/p19-w04-1_landing/doc/plan_phase-3.md)


### 목업 디자인 
Stitch, Gemini

![[p19-w04-1_mockup.png]]

> [!QUESTION] Gemini 디자인 요구사항 명세서
> - 제품 요구사항 명세서를 바탕으로 디자인 명세서 작성
> 	- (제품 요구사항 명세서 첨부)

> [!QUESTION] Stitch 목업 디자인
> - 디자인 요구사항 명세서를 바탕으로 웹디자인
> 	- (디자인 요구사항 명세서 내용 첨부)
> - 섹션별로 디자인 생성
> 	- 한국어
> 	- 인터랙티브 및 모션 요소 반영

> [!QUESTION] Gemini 디자인 섹션별 명세서 작성
> - 000 섹션 디자인 명세서 작성. 
> - 색상 코드와 폰트 정보 명세서 작성. 
> - 간격 및 정렬, 인터랙션 및 애니메이션, 접근성 및 SEO 명세서 작성.
> - (컬러 팔레트, 간격 및 정렬, 인터랙션 및 애니메이션, 접근성 및 SEO, 폰트 명세서 작성)


> [!EXAMPLE] 디자인 명세서
> - [섹션 1 - 히어로](https://github.com/knachinen/one-day-one-project/blob/main/p19-w04-1_landing/doc/design_section-1-hero.md)
> - 섹션 2 - 문제 제기
> - 섹션 3 - 솔루션 제시
> - 섹션 4 - 작동 방식
> - 섹션 5 - 라이브 데모
> - 섹션 6 - 성공 사례
> - 섹션 7 - 차별점 강조
> - 섹션 8 - 자주 묻는 질문
> - 섹션 9 - 커뮤니티 미리보기
> - 섹션 10 - 최종 전환 유도


### 작업 요청 
Gemini CLI

> [!QUESTION] 구현 프롬프트
> - 1단계 구현 (1단계 구현계획 및 관련 섹션 디자인 문서 첨부)
> - 2단계 구현 (2단계 구현계획 및 관련 섹션 디자인 문서 첨부)
> - 3단계 구현 (3단계 구현계획 및 관련 섹션 디자인 문서 첨부)


---

## 개발 과정 

### 구현 후 첫 실행

단계별로 구현 및 실행 검증을 함. 

### 구현 기능 검증

> [!BUG] 
> - `vibe-blue` 색상 적용이 안됨

### 수정 보완

> [!BUG] 
> - Hero, Header 디자인



---
## 결과 

![[p19-w04-1_screen.png]]

### 미완성

> [!BUG] 
> - 컬러 팔레트 적용 


### 완료

> [!SUCCESS] 
> - 목업 디자인을 바탕으로 한 기본적인 틀



---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p19-w04-1 - Landing](https://github.com/knachinen/one-day-one-project/tree/main/p19-w04-1_landing) (github.com)
