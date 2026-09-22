---
id: "2025-1129_6-333-48_213020"
date: "2025-11-29"
time: "2025-11-29T21:30:20"
tags: 
status: 
category:
description: 
---
---

## 개발 환경

- IDE : 반중력 편집기 (AntiGravity)
- 모델
	- 계획 (Planning) : Claude Sonnet 4.5
	- 구현 : Claude Sonnet 4.5, Gemini 3 Pro (Low)

---

## 프로젝트 아이템 

행동을 바탕으로 한 todo 앱을 만들어 보았다.  

---

## 작업 요청


> [!NOTE] 
> prd를 바탕으로 계획과 작업목록 작성. 문서만 작성.

Gemini 웹에서 PRD 를 만들고,  
이번에는 목업 디자인없이 진행했다.  


> [!EXAMPLE] 문서
> - [PRD](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/prd.md)
> - [Implementation Plan](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/implementation_plan.md)
> - [Task](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/task.md)
> - [Walkthrough](https://github.com/knachinen/one-day-one-project/blob/main/p06_w01-6_atomizer/doc/walkthrough.md)


---

## 개발 과정 

계획에 이어 클로드 소넷 4.5으로 구현을 진행했다.  

중간에 버그를 좀 고치기도 했고,  
기능이 좀 많아서 토큰을 다 소진했다.  

Gemini 3 Pro (Low) 모델로 이어서 구현을 마쳤다.  

---

## 결과 

역시나 오류.  
빌드부터가 안된다.  

### 오류 수정

빌드 오류를 고치느라 Gemini 3 Pro (Low) 토큰을 다 소진했다.  
Gemini 3 Pro (High) 로 바꿨는데, Low 모델과 토큰을 공유하는 것 같다.  
토큰이 없어서 사용하지 못했다.  

할 수 없이 젬씨 (Gemini CLI) 로 넘어왔다.  
지난한 과정을 지나서 겨우 앱이 실행되었다.  

빌드할 때 이상하다.  
첫번째 빌드 때는 빌드가 안되다가, 두번째는 또 된다.  
그 이유를 모르겠다.  

```bash
rm -rf node_modules package-lock.json && npm cache clean --force && npm install 
npx expo prebuild --clean 
rm -rf android/app/build 
npx expo run:android
```

젬씨가 코드 좀 수정한 뒤에 자꾸 초기화를 강요했다.  
혹시나해서 초기화없이 앱만 다시 로드했더니 에러가 고쳐지지 않았다.  

매번 초기화하느라 시간이 너무 많이 걸렸다.  

나중에 제미나이에게 다시 물어보니, 그럴 필요없... (아, 증말..)

그리고 코드 수정이 반영이 안되는 문제도 있었다.  
분명 편집기에서는 수정되었는데, 콘솔에서 코드를 확인하면 반영이 안되어있었다.  
왜 그런지 이유를 찾을 수 없는 가운데, 갑자기 반영되어 어리둥절했다.  

### 결과 감상 

![[p06-w01-6_screen-1.png|200]]
![[p06-w01-6_screen-2.png|200]]
![[p06-w01-6_screen-3.png|200]]
![[p06-w01-6_screen-4.png|200]]
발

---

## 깃헙 레포 


> [!INFO] 
> [p06_w01-6_atomizer](https://github.com/knachinen/one-day-one-project/tree/main/p06_w01-6_atomizer) (github.com)
