---
id: "2025-1202_2-336-49_204903"
date: "2025-12-02"
time: "2025-12-02T20:49:03"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] 프로젝트 아이템 
> - 간단한 PDF 뷰어 & 주석

---

## 개발환경

> [!INFO] IDE & 모델
> - IDE: 반중력편집기 (AntiGravity)
> - 모델
> 	- 계획: Gemini 3 Pro (High)
> 	- 구현: Gemini 3 Pro (High)
> 	- 디버깅: Gemini 3 Pro (High)

  

---

## 작업 요청

> [!QUESTION] 프롬프트
> - PRD 바탕으로 계획 및 작업목록 문서작성. 프로젝트 디렉토리는 'p09_w02-2_plainpdf' 사용.

어제 프로젝트에서 디렉토리명을 아무거나 쓰길래 지정해주었다.  

---

## 작업 문서 

> [!EXAMPLE] 문서
> - 제품명세서 : [PRD](https://github.com/knachinen/one-day-one-project/blob/main/p09_w02-2_plainpdf/doc/p09_w02-2_plainpdf.md)
> - 구현 계획 : [Implementation Plan](https://github.com/knachinen/one-day-one-project/blob/main/p09_w02-2_plainpdf/doc/implementation_plan.md)
> - 작업 목록 : [Task](https://github.com/knachinen/one-day-one-project/blob/main/p09_w02-2_plainpdf/doc/task.md)
> - 기술 검토 : [Walkthrough](https://github.com/knachinen/one-day-one-project/blob/main/p09_w02-2_plainpdf/doc/walkthrough.md)

---

## 개발 과정 

어제와 같이 리뷰 정책 `Always Proceed`, 터미널 커맨드 `Turbo` 로 구현은 금방 마무리되었다.  

---
## 결과 

![[p09-w02-2_plainpdf.png]]

> [!BUG] 
> - PDF 문서를 불러오지만, 내용이 보이지 않음.  -  해결됨  
> - 주석도구 (하이라이트, 텍스트, 펜) 기능이 동작하지 않음.  -  아직 해결되지 않음.  

> [!SUCCESS] 
> - 어제와는 다르게 적어도 앱은 켜진다.  
> - 몇 번의 디버깅으로 PDF 내용은 불러와졌다.  
> - 주석이 저장은 안되지만, 문서가 불러와져있는 동안은 기능한다.  



---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [P09_W02-2 프로젝트](https://github.com/knachinen/one-day-one-project/tree/main/p09_w02-2_plainpdf) (github.com)
