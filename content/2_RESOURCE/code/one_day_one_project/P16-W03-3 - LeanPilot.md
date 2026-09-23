---
id: "2025-1210_3-344-50_192215"
date: "2025-12-10"
time: "2025-12-10T19:22:15"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] LeanPilot
> - 제품 요구사항 명세서 가이드 템플릿 플랫폼

---

## 개발환경

> [!INFO] IDE & 모델
> - Gemini 2.5 Fast / Claude Sonnet 4.5 / ChatGPT / Grok Auto
> 	- 요구사항 명세서
> - Gemini CLI
> 	- 계획, 구현, 디버깅: Gemini 2.5 Auto, Flash


---

## 작업 요청

### 기획안 및 제품 요구사항 명세서 작성 
Gemini Fast, Claude Sonnet 4.5, ChatGPT, Grok Auto

> [!QUESTION] 프롬프트
> 다음 웹서비스 아이디어를 바탕으로 기획.
> 
> - 프로젝트 아이디어: 1인 기업가용 MVP 기획 템플릿 웹서비스 
> - 1인 기업의 관점 
> - '린 스타트업(Lean Startup)' 방법론에 기반 
> - MVP 아이데이션 및 개발 프로세스 
> - 템플릿을 따라 기획을 자연스럽게 유도
> 


> [!EXAMPLE] 기획안 및 제품 요구사항 명세서
> - Gemini : [PRD - Gemini](https://github.com/knachinen/one-day-one-project/blob/main/p16-w03-3_leanpilot/doc/gemini.md)
> - Claude : [PRD - Claude](https://github.com/knachinen/one-day-one-project/blob/main/p16-w03-3_leanpilot/doc/claude.md)
> - ChatGPT : [PRD - ChatGPT](https://github.com/knachinen/one-day-one-project/blob/main/p16-w03-3_leanpilot/doc/chatgpt.md)
> - Grok : [PRD - Grok](https://github.com/knachinen/one-day-one-project/blob/main/p16-w03-3_leanpilot/doc/grok.md)


### 목업 디자인 
Stitch


> [!QUESTION] Stitch 프롬프트
> - 기획안과 제품 요구사항 명세서를 바탕으로 웹디자인
> 	- (기획안 및 제품 요구사항 명세서 내용 첨부)

![[p16-w03-3_mockup.png]]

### 작업 요청 
Gemini CLI

> [!QUESTION] 반중력 프롬프트
> - 🔍  제품 요구사항 명세서를 개선점을 파악하고, 수정 보완하기. 
> - 📋  구현 계획, 구현 작업 목록 작성 


> [!EXAMPLE] 문서
> - 구현 계획 : [Implementation Plan](https://github.com/knachinen/one-day-one-project/blob/main/p15-w03-1_launchpad/doc/implementation_plan.md)
> - 작업 목록 : [Task](https://github.com/knachinen/one-day-one-project/blob/main/p15-w03-1_launchpad/doc/task_list.md)



---

## 개발 과정 

### Gemini CLI 사용

토큰을 다 소진해서 반중력을 쓸 수 없으므로,  
Gemini CLI 로 구현을 했다.  

### 구현 후 첫 실행

꽤 지난한 디버깅 끝에...
런칭을 할 수 있었다.

데이터베이스 오류를 수정하여 계정 생성과 로그인을 할 수 있게 되고,  
가이드 템플릿에 따라 겨우 문서를 작성할 수 있게 되었다.  

그럼에도 완전히 작성이 되지는 않고 몇몇 오류가 남아있다.  

> [!BUG] 
> - 런칭 
> - 데이터베이스 
> - 스테이지 페이지 (가이드 템플릿 문서 작성)

### 구현 기능 검증

> [!BUG] 
> - (추후 업데이트 예정)


### 수정 보완

> [!BUG] 
> - (추후 업데이트 예정)



---
## 결과 

![[p16-w03-3_screen.png]]

> [!SUCCESS] 
> - 계정 생성 및 로그인/로그아웃
> - 프로젝트 생성
> - 가이드 템플릿 문서 작성



---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p16_w03-3_LeanPilot](https://github.com/knachinen/one-day-one-project/tree/main/p16-w03-3_leanpilot) (github.com)
