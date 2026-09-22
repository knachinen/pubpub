---
id: "2025-1130_0-334-49_221307"
date: "2025-11-30"
time: "2025-11-30T22:13:07"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] 오늘 되돌아보기
> - 매일 3개의 질문으로 하루를 되돌아보기

---

## 개발환경

> [!INFO] IDE & 모델
> - IDE: 반중력편집기 (AntiGravity)
> - 모델
> 	- 계획: Claude Sonnet 4.5
> 	- 구현: Gemini 3 Pro (High)

이번에는 구현을 Gemini 3 Pro (High) 로 해보기로 했다.  
프로젝트에 따라 토큰이 얼마나 소모되는지 확인해보고 싶었다.  

결과적으로 이 정도 프로젝트에서는 토큰제한에 걸리지 않고 구현이 되었다.  

---

## 작업 요청

> [!QUESTION] 프롬프트
> prd를 바탕으로 계획과 작업목록 작성. 문서만 작성.

---

## 작업 문서 

> [!EXAMPLE] 문서
> - 제품명세서 : [PRD](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/prd.md)
> - 구현 계획 : [Implementation Plan](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/implementation_plan.md)
> - 작업 목록 : [Task](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/task.md)
> - 기술 검토 : [Walkthrough](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/walkthrough.md)

---

## 개발 과정 

![[antigravity_settings_artifact.png]]

지금까지는 `Request Review` 로 썼었는데,  알아서 진행하도록 해봤다.  

![[antigravity_terminal_command_options.png]]

터미널 커맨드 옵션도 그냥 다 실행하도록 설정했다.  

그 결과로 알아서 다 구현하고 다 실행되었다.  

---
## 결과 

![[p07-w01-7_refelectly.png]]

> [!BUG] 
> - 모바일 디바이스 알림 관련 에러

> [!SUCCESS] 
> - 큰 오류없이 실행됨

아주 가뿐하게 금방 만들어졌다.  `딸깍`  

Claude Sonnet 4.5 모델로 구현한 것보다 결과가 더 좋아보인다.  
게다가 큰 에러도 발생하지 않았다.  

앞으로 당분간은 토큰 사용량을 살펴볼겸 `Gemini 3 Pro (High)` 로 써봐야겠다.  
계획 품질도 다를까?  
처음에 써볼 때, **글래스 모피즘** 디자인을 적용했던 것을 보면 다를 것으로 예상된다.  


---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p07_w01-7_reflectly](https://github.com/knachinen/one-day-one-project/tree/main/p07_w01-7_reflectly) (github.com)
