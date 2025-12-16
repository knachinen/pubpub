---
id: "2025-1216_2-350-51_205452"
date: "2025-12-16"
time: "2025-12-16T20:54:52"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] 랜딩페이지 시리즈 - 메모앱
> - 메모앱 랜딩페이지

---

## 개발환경

> [!INFO] IDE & 모델
> - Gemini 2.5 Fast / **Claude** Sonnet 4.5 / **ChatGPT** / Grok Auto
> 	- 기획안 및 제품 요구사항 명세서 작성
> - Google Stitch
> 	- 목업 디자인
> - Gemini CLI
> 	- 계획, 구현, 디버깅: Gemini 2.5 Flash


---

## 작업 요청

### 기획안 및 제품 요구사항 명세서 작성 
Gemini Fast, Claude Sonnet 4.5, ChatGPT, Grok Auto

> [!QUESTION] 프롬프트: 기획안
> - 메모앱 랜딩페이지 기획안 작성

> [!EXAMPLE] 기획안 
> - [Gemini](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_gemini.md)
> - [Claude](hhttps://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_claude.md)
> - [ChatGPT](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_chatgpt.md)
> - [Grok](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_grok.md)

> [!QUESTION] 프롬프트: 제품 요구사항 명세서, 기술 스택, 단계별 구현 계획
> - 제품 요구사항 명세서 작성
> - 단계별 구현 계획 작성. 단계별로 독립적인 실행이 가능해야 함. 


> [!EXAMPLE] 최종 기획안, 제품 요구사항 명세서
> - [최종 기획안](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_merged) : Claude + ChatGPT
> - [제품 요구사항 명세서](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_prd) : Claude

### 목업 디자인 
Stitch, Gemini

![[p20-w04-2_mockup.png|500]]

> [!QUESTION] Stitch 목업 디자인
> - 기획안과 제품 요구사항 명세서를 바탕으로 웹디자인
> 	- (기획안 및 제품 요구사항 명세서 내용 첨부)

> [!EXAMPLE] 목업 디자인용 기획안 
> - [목업 디자인용 기획안](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_prd-for-design.md)

> [!QUESTION] ChatGPT 디자인 명세서 작성
> - 000 섹션 디자인 상세 명세서 작성. 

오늘은 ChatGPT 를 사용해봄.  
내용이 Gemini 보다 더 나아보였음.  

> [!EXAMPLE] 디자인 명세서 : ChatGPT
> - [섹션 1 - 히어로](https://github.com/knachinen/one-day-one-project/blob/main/p20-w04-2_landing-memo/doc/design_section-1-hero.md)

모든 섹션을 완성하는 게 목적이 아니므로,  
시간을 아낄겸 섹션1 히어로만 구현하기로 함.  

### 작업 요청 
Gemini CLI


> [!QUESTION] 구현 프롬프트 : ChatGPT
> - 단계별 구현 계획 작성. 단계별로 독립적인 실행이 가능해야 함. 가능한 작은 단계로 나눌 것.

`Phase 7. Use Case` 섹션까지 작성을 해주었지만,  
히어로 섹션만 만들 예정이므로,  
Phase 4. 기본모션까지만 구현.  

> [!EXAMPLE] 단계별 구현계획
> - [단계별 구현계획](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_implement.md)
> 	- [1단계 구현계획](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_implement-01.md) : Phase 0
> 	- [2단계 구현계획](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_implement-02.md) : Phase 1
> 	- [3단계 구현계획](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_implement-03.md) : Phase 2
> 	- [4단계 구현계획](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_implement-04.md) : Phase 3
> 	- [5단계 구현계획](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo/doc/plan_implement-05.md) : Phase 4



---

## 개발 과정 

### 구현 후 첫 실행

단계별로 구현 및 실행 검증을 함. 

### 구현 기능 검증

> [!BUG] 
> - 모션 적용이 안됨

시스템에서 `Reduce Motion` 적용이 되어있기 때문.  
개발모드에서는 무시하는 방법을 쓰려고 했는데, 잘 안되어서 그냥 시스템 환경설정을 바꿈.  

### 수정 보완

> [!BUG] 
> - 히어로 섹션 디자인 상세 명세서 적용



---
## 결과 


![[p20-w04-2_screen.png|500]]

### 미완성

> [!BUG] 
> - 목업 이미지와 다른점들 
> - 히어로 섹션 외 나머지 섹션들


### 완료

> [!SUCCESS] 
> - 대부분의 구현 계획
> - 목업 디자인 적용



---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p20-w04-2 - Landing - MemoApp](https://github.com/knachinen/one-day-one-project/tree/main/p20-w04-2_landing-memo) (github.com)
