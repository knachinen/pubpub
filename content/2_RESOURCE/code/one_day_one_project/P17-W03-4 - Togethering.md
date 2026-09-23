---
id: "2025-1211_4-345-50_104754"
date: "2025-12-11"
time: "2025-12-11T10:47:54"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] Togethering
> - 소규모 그룹 프로젝트 관리

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
> - 다음 웹서비스 아이디어를 바탕으로 기획.>   
> 	- 프로젝트 아이디어: 소규모 그룹 프로젝트 및 일정 관리
> 	- 대상: 커플, 소규모 그룹 (2~4명)
> 	- 기능: 그룹 내 프로젝트, 일정, 이벤트 관리


> [!EXAMPLE] 기획안 및 제품 요구사항 명세서
> - Gemini : [PRD - Gemini](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/gemini.md)
> - Claude : [PRD - Claude](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/claude.md)
> - ChatGPT : [PRD - ChatGPT](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/chatgpt.md)
> - Grok : [PRD - Grok](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/grok.md)

### 목업 디자인 
Stitch

![[p17-w03-4_mockup.png]]

> [!QUESTION] Stitch 프롬프트
> - 기획안과 제품 요구사항 명세서를 바탕으로 웹디자인
> 	- (기획안 및 제품 요구사항 명세서 내용 첨부)

### 목업 디자인 명세서
Gemini

> [!EXAMPLE] 문서
> - [캘린더](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/design_calendar.md)
> - [대시보드](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/design_dashboard.md)
> - [로그인](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/design_log-in.md)
> - [그룹 생성](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/design_new-group.md)
> - [프로젝트 생성](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/design_new-project.md)
> - [온보딩](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/design_on-boarding.md)
> - [프로젝트 관리](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/design_project.md)


### 작업 요청 

> [!QUESTION] 단계별 구현 계획 작성
> - 📋 [1 단계](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/phase-01.md)
> - 📋 [2 단계](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/phase-02.md)
> - 📋 [3 단계](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/phase-03.md)
> - 📋 [4 단계](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/phase-04.md)
> - 📋 [5 단계](https://github.com/knachinen/one-day-one-project/blob/main/p17-w03-4_togethering/doc/phase-05.md)

---

## 개발 과정 

### 구현 기능 검증

> [!BUG] 
> - 계정 생성 및 로그인
> - 데이터베이스 연결
> - 그룹 및 프로젝트 생성
> - 프로젝트 내 할 일 관리 (칸반보드)

기본적으로 거의 모든 링크가 연결되어 있지 않았다.  
기능은 구현을 했는데, 내비게이션 링크가 되어있지 않아서 하나씩 다 요청을 해야했다.  

중간에 갑자기 테마를 다크모드로 변경이 되었는데,  
이렇게 된 김에 테마를 선택할 수 있게 하려고 했다.  
그렇게 무한 디버깅 속으로...  
코드를 되돌리고 라이트모드로 하나씩 변경했다.  

디자인 명세서를 시험삼아 적용해봤는데, 결과가 썩 좋지 않고,  
또 오류가 잔뜩 생겨나서 시간상 코드를 되돌렸다.  

---
## 결과 

![[p17-w03-4_screen.png]]

---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p17_w03-4_Togethering](https://github.com/knachinen/one-day-one-project/tree/main/p17-w03-4_togethering) (github.com)
