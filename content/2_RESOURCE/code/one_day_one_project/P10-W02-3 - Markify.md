---
id: "2025-1203_3-337-49_200200"
date: "2025-12-03"
time: "2025-12-03T20:02:00"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] 프로젝트 아이템 
> - 웹문서 마크다운 문서 아카이브

---

## 개발환경

> [!INFO] IDE & 모델
> - IDE: 반중력편집기 (AntiGravity)
> - 모델
> 	- 계획: Gemini 3 Pro (High)
> 	- 구현: Gemini 3 Pro (High)
> 	- 디버깅: Gemini 3 Pro (High), Claude Sonnet 4.5, Gemini CLI

  

---

## 작업 요청

> [!QUESTION] 프롬프트
> - PRD 바탕으로 계획 및 작업목록 문서작성.

---

## 작업 문서 

> [!EXAMPLE] 문서
> - 제품명세서 : [PRD](https://github.com/knachinen/one-day-one-project/blob/main/p10_w02-3_markify/doc/p10_w02-3_markify.md)
> - 구현 계획 : [Implementation Plan](https://github.com/knachinen/one-day-one-project/blob/main/p10_w02-3_markify/doc/implementation_plan.md)
> - 작업 목록 : [Task](https://github.com/knachinen/one-day-one-project/blob/main/p10_w02-3_markify/doc/task.md)
> - 기술 검토 : [Walkthrough](https://github.com/knachinen/one-day-one-project/blob/main/p10_w02-3_markify/doc/walkthrough.md)

---

## 개발 과정 


> [!NOTE] 
> - 리뷰 정책 : `Always Proceed`
> - 터미널 커맨드 : `Turbo`


---
## 결과 

![[p10-w02-3_markify.png]]

> [!BUG] 
> - share 
> - assembleRelease 

> [!SUCCESS] 
> - 웹브라우저에서 자바스크립트로 html 전달 
> - 마크다운 프리뷰 / 편집 / 저장 / 복사 

대략 몇 번 디버깅 끝에 앱은 실행되었다.  

처음에는 웹주소로 html 컨텐츠를 받아온 뒤,  
마크다운 문서로 변환하려고 했다.  

CORS 때문에 html 컨텐츠를 가져올 수 없어서,  
웹브라우저에서 html 을 전달하는 방법으로 변경했다.  
이에 따라 UI 도 바꾸었다.  

나름 쓸만해서 디바이스에 정식으로 설치를 하려고 했다.  
개발 빌드에서는 되던 게 릴리즈 빌드에서는 실패했다.  

Gemini 3 Pro (High) 에서 Claude Sonnet 4.5로,  
그것도 모자라 Gemini CLI 로 넘어와서까지,  
지난한 디버깅 끝에 시간이 없어서 포기를 했다.  

---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [P10-W02-3_Markify](https://github.com/knachinen/one-day-one-project/tree/main/p10_w02-3_markify) (github.com)
