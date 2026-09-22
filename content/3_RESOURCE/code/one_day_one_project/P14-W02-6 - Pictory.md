---
id: "2025-1206_6-340-49_205111"
date: "2025-12-06"
time: "2025-12-06T20:51:11"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] Pictory
> - 이미지 및 짧은 글 공유 커뮤니티 웹서비스

---

## 개발환경

> [!INFO] IDE & 모델
> - Gemini 2.5 Fast
> 	- 실현가능성
> 	- 요구사항 명세서
> - 반중력편집기 (AntiGravity)
> 	- 요구사항 명세서 리뷰: Gemini 3 Pro (High)
> 	- 계획: Gemini 3 Pro (High)
> 	- 구현: Gemini 3 Pro (High)
> - Gemini CLI
> 	- 디버깅: Gemini 2.5 Flash


---

## 작업 요청

### 실현 가능성 검토 (Gemini Web)

> [!QUESTION] Gemini 프롬프트
> - 프로젝트 : 인스타그램 같은 이미지 및 짧은 글 공유 커뮤니티 웹서비스 제품 요구사항 명세서 작성.


> [!EXAMPLE] 문서
> - 제품명세서 : [PRD](https://github.com/knachinen/one-day-one-project/blob/main/p14_w02-6_pictory/doc/prd.md)



### 목업 디자인 (Stitch)

> [!QUESTION] Stitch 프롬프트
> - PRD 바탕으로 앱 디자인
> 	- (PRD 답변 첨부)

![[p14-w02-6_mockup.png]]


### 작업 요청 (반중력)

> [!QUESTION] 반중력 프롬프트
> - 🔍  제품 요구사항 명세서를 개선점을 파악하고, 수정 보완하기. 문서만 업데이트하고 지시 기다릴것.
> - 📱  목업 디자인 요구사항 정리
> - 📋  구현 계획, 구현 작업 목록 작성 
> - ▶️  문서 작성 후 구현 자동 시작


> [!EXAMPLE] 문서
> - 디자인 요구사항 정리 : [Design](https://github.com/knachinen/one-day-one-project/blob/main/p14_w02-6_pictory/doc/design.md)
> - 구현 계획 : [Implementation Plan](https://github.com/knachinen/one-day-one-project/blob/main/p14_w02-6_pictory/doc/implementation_plan.md)
> - 작업 목록 : [Task](https://github.com/knachinen/one-day-one-project/blob/main/p14_w02-6_pictory/doc/task.md)
> - 기술 검토 : [Walkthrough](https://github.com/knachinen/one-day-one-project/blob/main/p14_w02-6_pictory/doc/walkthrough.md)

---

## 개발 과정 


> [!BUG] 
> - TypeError [ERR_UNKNOWN_FILE_EXTENSION]: Unknown file extension ".ts"`

디버깅이 되지 않았다.  
이렇게 저렇게 수정하다보니, 결국 무한 루프로 수정을 하고 있었다.  

Next.js 로 코드를 뜯어 고쳤다.  


Gemini 가 작성한 기술스택이 좀 별로여서,  
Claude 와 ChatGPT, Grok 버전도 만들어봤다.  

> [!EXAMPLE] 문서
> - 제품명세서 (클로드 소넷 4.5) : [PRD - Claude](https://github.com/knachinen/one-day-one-project/blob/main/p14_w02-6_pictory/doc/prd_claude.md)
> - 제품명세서 (챗GPT) : [PRD - ChatGPT](https://github.com/knachinen/one-day-one-project/blob/main/p14_w02-6_pictory/doc/prd_chatgpt.md)
> - 제품명세서 (챗GPT) : [PRD - ChatGPT](https://github.com/knachinen/one-day-one-project/blob/main/p14_w02-6_pictory/doc/prd_grok.md)

클로드가 작성한 명세서의 기술 스택이 가장 낫다.  
다음에는 비교를 좀 한 뒤에, 괜찮은 것으로 골라야겠다.  


> [!SUCCESS] 
> - 계정 등록 및 로그인 

Next.js 로 수정한 뒤, 계정을 등록하고 로그인은 되었다.  
하지만...  
젬씨가 Next.js 로 변경하는 과정에서 거의 초기화 수준으로 만들어 놓은듯하다.  

![[p14-w02-6_login.png]]

---
## 결과 


> [!SUCCESS] 
> - ...지난한 과정 끝에 계정 등록 및 로그인은 됨. 

이 프로젝트는 다시 만들어야할 것 같다.  

---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p14_w02-6_Pictory](https://github.com/knachinen/one-day-one-project/tree/main/p14_w02-6_pictory) (github.com)
