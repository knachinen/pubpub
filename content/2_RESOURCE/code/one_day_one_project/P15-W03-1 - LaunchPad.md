---
id: "2025-1208_1-342-50_171448"
date: "2025-12-08"
time: "2025-12-08T17:14:48"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] LaunchPad 
> - 아이디어/MVP 공유 및 피드백 웹서비스

---

## 개발환경

> [!INFO] IDE & 모델
> - Gemini 2.5 Fast / Claude Sonnet 4.5 / ChatGPT / Grok Auto
> 	- 요구사항 명세서
> - 반중력편집기 (AntiGravity)
> 	- 요구사항 명세서 리뷰: Gemini 3 Pro (High)
> 	- 계획: Gemini 3 Pro (High)
> 	- 구현: Gemini 3 Pro (High)
> - Gemini CLI
> 	- 디버깅: Gemini 2.5 Auto, Flash


---

## 작업 요청

### 기획안 및 제품 요구사항 명세서 작성 
Gemini Fast, Claude Sonnet 4.5, ChatGPT, Grok Auto

> [!QUESTION] 프롬프트
> - 인스타그램 같은 이미지 및 짧은 글 공유 커뮤니티 웹서비스 제품 요구사항 명세서 작성.
> - MVP 기술스택은 클라우드 서비스없이 로컬환경에 맞게 변경. 기술스택 최신 버전으로 맞추기.


> [!EXAMPLE] 기획안 및 제품 요구사항 명세서
> - Gemini : [PRD - Gemini](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/prd.md)
> - Claude : [PRD - Claude](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/prd.md)
> - ChatGPT : [PRD - ChatGPT](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/prd.md)
> - Grok : [PRD - Grok](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/prd.md)


### 목업 디자인 
Stitch


> [!QUESTION] Stitch 프롬프트
> - 기획안과 제품 요구사항 명세서를 바탕으로 웹디자인
> 	- (기획안 및 제품 요구사항 명세서 내용 첨부)

![[p15-w03-1_mockup.png]]

### 작업 요청 
반중력

> [!QUESTION] 반중력 프롬프트
> - 🔍  제품 요구사항 명세서를 개선점을 파악하고, 수정 보완하기. 
> - 📱  목업 디자인 요구사항 명세서 작성.  
> - 📋  구현 계획, 구현 작업 목록 작성 
> - ▶️  문서 작성 후 구현 자동 시작


> [!EXAMPLE] 문서
> - 디자인 요구사항 : [Design](https://github.com/knachinen/one-day-one-project/blob/main/p15-w03-1_launchpad/doc/design.md)
> - 구현 계획 : [Implementation Plan](https://github.com/knachinen/one-day-one-project/blob/main/p15-w03-1_launchpad/doc/implementation_plan.md)
> - 작업 목록 : [Task](https://github.com/knachinen/one-day-one-project/blob/main/p15-w03-1_launchpad/doc/task.md)
> - 기술 검토 : [Walkthrough](https://github.com/knachinen/one-day-one-project/blob/main/p15-w03-1_launchpad/doc/walkthrough.md)


---

## 개발 과정 

### 반중력 토큰 소진

토큰 정책이 바뀌면서 페이즈2 구현 중에 토큰이 모두 소진되었다.  
4일 뒤 금요일에 초기화된다.  
할 수 없이 Gemini CLI 로 넘어와 구현을 마쳤다. 

### 구현 후 첫 실행

![[p15-w03-1_screen.png]]

일단 계정 생성과 로그인은 된다.  
하지만 아이디어 등록이나 메이커 정보는 보이지 않았다.  

시간상 이 프로젝트는 나중에 이어서 해야겠다. 

> [!BUG] 
> - (추후 업데이트 예정)

```bash

```

### 구현 기능 검증

> [!BUG] 
> - (추후 업데이트 예정)


### 수정 보완

> [!BUG] 
> - (추후 업데이트 예정)



---
## 결과 

> [!SUCCESS] 
> - 랜딩 페이지
> - 계정 생성 및 로그인



---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p15_w03-1_LaunchPad](https://github.com/knachinen/one-day-one-project/tree/main/p15-w03-1_launchpad) (github.com)
