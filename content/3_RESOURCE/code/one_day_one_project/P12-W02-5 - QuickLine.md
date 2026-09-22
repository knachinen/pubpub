---
id: "2025-1205_5-339-49_104903"
date: "2025-12-05"
time: "2025-12-05T10:49:03"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] 긴급 연락
> - 긴급 상황에서 빠르게 지인에게 연락하기

---

## 개발환경

> [!INFO] IDE & 모델
> - IDE: 반중력 (AntiGravity) 편집기
> 	- 계획: Gemini 3 Pro (High)
> 	- 구현: Gemini 3 Pro (High)
> - 디버깅: Gemini CLI


---

## 작업 요청

### 목업 디자인

![[p12-w02-5_mockup.png]]


### 작업 요청 


> [!QUESTION] 프롬프트
> - PRD 를 검토하여 개선사항을 수정 및 보완 
> - (목업 디자인 첨부) 위 목업 디자인을 참고로 하여 앱을 디자인


---

## 작업 문서 

> [!EXAMPLE] 문서
> - 실현가능성 검토 : [Feasibility](https://github.com/knachinen/one-day-one-project/blob/main/p12_w02-5_quickline/doc/feasibility.md)
> - 제품명세서 : [PRD](https://github.com/knachinen/one-day-one-project/blob/main/p12_w02-5_quickline/doc/prd.md)
> - 구현 계획 : [Implementation Plan](https://github.com/knachinen/one-day-one-project/blob/main/p12_w02-5_quickline/doc/implementation_plan.md)
> - 작업 목록 : [Task](https://github.com/knachinen/one-day-one-project/blob/main/p12_w02-5_quickline/doc/task.md)
> - 기술 검토 : [Walkthrough](https://github.com/knachinen/one-day-one-project/blob/main/p12_w02-5_quickline/doc/walkthrough.md)

---

## 개발 과정 

- 목업 이미지에 112, 119 버튼이 있어서, 구현 계획에서도 따르고 있음.  
- 문서를 한글로 작성했다가, 영문으로 작성했다가 오락가락함. 처음에 지정해줘야할듯. 
- 반중력 토큰정책이 바뀌어서 구현 뒤 디버깅, 수정은 Gemini CLI 로 진행했다. 
- 전화 및 문자 메시지는 정책상 직접적으로 할 수 없었다. 
- 디스코드 메시지 보내는 방법을 추가했다. 

---
## 결과 

![[p12-w02-5_screen.png]]


> [!BUG] 
> - 대체적으로 몇 번의 디버깅 끝에 수정되었다. 

> [!SUCCESS] 
> - 연락처 수정 
> - 디스코드 메시지 옵션 추가. 
> 	- 웹훅 설정
> - 연락 설정에 따른 버튼 활성/비활성화



---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [P12_W02-5_QuickLine](https://github.com/knachinen/one-day-one-project/tree/main/p12_w02-5_quickline/) (github.com)
