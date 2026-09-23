---
id: "2025-1217_3-351-51_190220"
date: "2025-12-17"
time: "2025-12-17T19:02:20"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] Kkobagi 
> - 습관 트래킹 

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
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p21_w04-3_Kkobagi](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/) (github.com)

---

## 작업 요청

### 기획안 및 제품 요구사항 명세서 작성 
Gemini Fast, Claude Sonnet 4.5, ChatGPT, Grok Auto

> [!QUESTION] 프롬프트: 기획안
> - 습관 형성 챌린지 웹플랫폼 기획안 작성
> 	- 인터랙티브, 애니메이션, 모션 요소
> 	- 대시보드
> 	- 톤앤매너: 친근함

> [!EXAMPLE] 기획안 
> - [Gemini](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/1-plan__gemini.md)
> - [Claude](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/1-plan__claude.md)
> - [ChatGPT](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/1-plan__chatgpt.md)
> - [Grok](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/1-plan__grok.md)

> [!QUESTION] 프롬프트: 제품 요구사항 명세서, 기술 스택, 단계별 구현 계획
> - 제품 요구사항 명세서 작성
> - 단계별 구현 계획 작성. 단계별로 독립적인 실행이 가능해야 함. 


> [!EXAMPLE] 최종 기획안, 제품 요구사항 명세서
> - [최종 기획안](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/1-plan__gemini.md) : Gemini
> - [제품 요구사항 명세서](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/2-prd__selected.md) : Claude


### 목업 디자인 
Stitch, Gemini

![[p21-w04-3_mockup.png]]

> [!QUESTION] Stitch 목업 디자인
> - 제품 요구사항 명세서를 바탕으로 웹디자인
> 	- (제품 요구사항 명세서 내용 첨부)

> [!QUESTION] Gemini, ChatGPT 디자인 명세서 작성
> - 목업 디자인을 바탕으로 상세 디자인 명세서 작성. 

오늘은 Gemini.  
ChatGPT, Gemini 두 개로 만들었는데,  
디자인의 디테일이 Gemini 가 더 나은 것 같았음.  

어제는 맥락을 반영하려고 제품 요구사항 명세서 작성 채팅에서 작업을 했음.  
어제 결과를 보니 목업 디자인과 좀 많이 다른 것 같아서,  
목업 디자인에 더 가깝게 하라는 뜻에서 따로 작업함.  

> [!EXAMPLE] 디자인 명세서 : ChatGPT
> - [섹션 1 - 대시보드 (Gemini)](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/3-design-1__gemini.md)
> - [섹션 1 - 대시보드 (ChatGPT)](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/3-design-1__chatgpt.md)
> - [섹션 2 - 습관 추가](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/3-design-2__gemini.md)
> - [섹션 1 - 습관 추가](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/3-design-2__chatgpt.md)


### 작업 요청 
Gemini CLI


> [!QUESTION] 구현 프롬프트 : ChatGPT
> - 단계별 구현 계획 작성. 단계별로 독립적인 실행이 가능해야 함. 가능한 작은 단계로 나눌 것.


> [!EXAMPLE] 단계별 구현계획
> - [단계별 구현계획](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/4-phase__gemini.md)
> 	- [1단계 구현계획](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/4-phase-1__gemini.md) : Phase 1
> 	- [2단계 구현계획](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/4-phase-2__gemini.md) : Phase 2
> 	- [3단계 구현계획](https://github.com/knachinen/one-day-one-project/tree/main/p21-w04-3_kkobagi/doc/4-phase-3__gemini.md) : Phase 3


---

## 개발 과정 

### 구현 후 첫 실행

단계별로 구현 및 실행 검증을 함. 

### 구현 기능 검증

> [!BUG] 
> - ui state : 체크했다가 취소를 하면 상태값이 엉킴. 화면에서는 취소되었지만, 실제는 체크된 상태.

### 수정 보완

> [!BUG] 
> - 목업 디자인 재적용



---
## 결과 

![[p21-w04-3_screen.png]]

### 미완성

> [!BUG] 
> - 습관 체크 상태 


### 완료

> [!SUCCESS] 
> - 대부분의 구현 계획
> - 목업 디자인 적용


## 리뷰

목업 디자인을 재적용했지만, 차이가 큼.  
이전에 목업 디자인을 먼저 구현했을 때 비슷했음.  
다음에는 레이아웃을 구현하고,  
기능을 구현해보겠음.  


