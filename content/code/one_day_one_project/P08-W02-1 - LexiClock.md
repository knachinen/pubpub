---
id: "2025-1201_1-335-49_213316"
date: "2025-12-01"
time: "2025-12-01T21:33:16"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] 알파벳 시계
> - 알파벳으로 시간을 표시

---

## 개발환경

> [!INFO] IDE & 모델
> - IDE: 반중력편집기 (AntiGravity)
> - 모델
> 	- 계획: Claude Sonnet 4.5
> 	- 구현: Gemini 3 Pro (High)

  

---

## 작업 요청

> [!QUESTION] 프롬프트
> - 기획안과 PRD 바탕으로 개발 계획 및 작업목록 작성.

---

## 작업 문서 

> [!EXAMPLE] 문서
> - 기획안 및 제품명세서 : [PRD](https://github.com/knachinen/one-day-one-project/blob/main/p08_w02-1_lexiclock/doc/p08_w02-1_lexiclock.md)
> - 구현 계획 : [Implementation Plan](https://github.com/knachinen/one-day-one-project/blob/main/p08_w02-1_lexiclock/doc/implementation_plan.md)
> - 작업 목록 : [Task](https://github.com/knachinen/one-day-one-project/blob/main/p08_w02-1_lexiclock/doc/task.md)
> - 기술 검토 : [Walkthrough](https://github.com/knachinen/one-day-one-project/blob/main/p08_w02-1_lexiclock/doc/walkthrough.md)

---

## 개발 과정 

리뷰 정책 `Always Proceed`, 터미널 커맨드 `Turbo` 로 구현은 금방 되었다.  

---
## 결과 


> [!BUG] 
> ERROR [TypeError: Cannot read property 'S' of undefined]  
> ERROR [TypeError: Cannot read property 'default' of undefined]  
> ERROR [TypeError: Cannot read property 'S' of undefined]  
> ERROR [TypeError: Cannot read property 'default' of undefined]  

패키지 버전 충돌이 문제인 것 같다.  
결국 Gemini 3 Pro (High), Claude Sonnet 4.5 모델 모두 문제를 해결하지 못했다.  

수동으로 디버깅을 해야할 것 같다.  
일단 오늘은 시간이 부족해서 여기서 마무리했다.  

---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p08_w02-1_프로젝트](https://github.com/knachinen/one-day-one-project/tree/main/p08_w02-1_lexiclock) (github.com)
