---
id: "2025-1218_4-352-51_220720"
date: "2025-12-18"
time: "2025-12-18T22:07:20"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] P20-W04-2 재구현
> - 목업 디자인에 가깝게 구현해보기

---

## 개발환경

> [!INFO] IDE & 모델
> - Gemini CLI
> 	- 계획, 구현, 디버깅: Gemini 2.5 Auto, Flash

---

## 작업 요청

### 기획안 및 제품 요구사항 명세서 작성 
Gemini Fast, Claude Sonnet 4.5, ChatGPT, Grok Auto

> [!NOTE] 이전 블로그 참조
> [[P20-W04-2 - Landing - Memo]]

### 목업 디자인 
Stitch, Gemini

![[p20-w04-2_mockup.png|500]]

### 작업 요청 
Gemini CLI


> [!EXAMPLE] 구현 프롬프트
> [@doc/5-impl-start.md](https://github.com/knachinen/one-day-one-project/blob/main/p22-w04-4_landing-memo-2/doc/5-impl-start.md)

PRD, 테크스택, 디자인 명세서, 구현 계획 개요, 구현 상세 계획 - 페이즈 1 문서를 참조하게 하고,  
요청 사항에는 다음과 같이 작성했다.  

> - 참고 문서를 읽을 것
> - 테크스택과 함께 디자인 명세서를 구현하기 위한 할일목록을 작성
> - 할일목록을 파일로 저장
> - 스텝 바이 스텝으로 할일목록 레이아웃을 구현
> - 한 스텝 끝나면 내가 검증할 것

---

## 개발 과정 

색상 설정이 잘 안되었다.  
[Tailwind CSS v4 릴리즈](https://tailwindcss.com/blog/tailwindcss-v4) 날짜가 2025년 1월 22일.  
젬니 2.5 모델이 학습이 안되어서 그런지 잘 수정하지 못하다가,  
웹검색 해보라고 하고 나서야 수정이 되었다.  

> [!BUG] 
> Tailwind CSS v4 defines custom colors in globals.css via @theme, not tailwind.config.ts. That's why my primary color wasn't working. My plan is to remove extend.colors from tailwind.config.ts and define primary and primary-dark in src/app/globals.css using @theme and CSS variable naming. First, modify tailwind.config.ts.

> [!BUG] 
>  globals.css is updated with custom colors via @theme. I'll ask the user to restart the dev server to verify the text-primary and bg-primary colors are now
  correctly applied to the button and auxiliary message.

> [!BUG] 
> I have updated tailwind.config.ts by removing the colors extension and defined the custom primary and primary-dark colors in src/app/globals.css using the
  @theme directive, as required by Tailwind CSS v4.


---
## 결과 

![[p22-w04-4_screen.png|500]]

저번에 구현된 결과와 비교해보자.  

![[p20-w04-2_screen.png|500]]

생각으로는 디자인 레이아웃을 중심으로 구현을 하면,  
좀 더 목업 디자인에 가깝게 될 줄 알았는데,  
꼭 그렇지만도 않다.  

일단 색상은 명세서에 맞게 라벤더 색상으로 되었다.  
버튼도 잘 만들어졌다.  

카드 내용이 이전보다 질이 낮고,  
위치 설정도 잘 안되었다.  
배경도 이전에는 동적으로 변했는데,  
이번에는 배경설정도 하지 않았다.  

게다가 실망스러운건 이렇게 구현하는데도,  
2시간 넘게 걸렸다는거다.  
물론 스텝별로 검증하느라 시간이 걸리긴 했지만,  
생각보다 너무 많이 걸렸다.  

디자인 명세서가 상세하게 기술되지 않아서일까?  

> - **배경**: 소프트 컬러 그라데이션이 부드럽게 움직이는 애니메이션 적용 (기획안 기반).
> - **UI 카드**: **글래스모피즘** 스타일 적용 (반투명 배경, 블러 효과).
> - **데모 카드**: 마우스 커서를 따라 움직임.

적어도 위 내용은 [할일목록](https://github.com/knachinen/one-day-one-project/blob/main/p22-w04-4_landing-memo-2/doc/todo_list.md)에 반영되지 않았다.  
할일목록에 디자인 명세서 내용이 좀 더 반영될 수 있게 만들어야겠다.  

---

## 개선

### 1차 개선

> [!QUESTION] 1차 개선 프롬프트
> (1차 개선 문서 첨부) 목업 디자인과 결과에 차이가 있음. 개선할 것.

![[p22-w04-4_screen_imprv-1.png|500]]

### 2차 개선

> [!QUESTION] 2차 개선 프롬프트
> (2차 개선 문서 첨부) 문서 리뷰. 레이아웃 코드로 리팩토링할 것. (하드코딩하지 말것)

![[p22-w04-4_screen_improvement-2.png|500]]

### 바이브코딩 플랫폼 비교

Lovable

![[p22-w04-4_screen_lovable.png|500]]

와... 놀랬다.  
순식간에 이런 페이지가 만들어졌다.  
목업이미지처럼 헤더를 구현해냈다.  

Base44

![[p22-w04-4_screen_base44.png|500]]

Lovable 보다는 별로지만 나쁘지않다.  
실행하자마자 뭐가 뜨길래 뭔가 했는데 이미 작업이 끝난거였다.  
속도면에서 놀랐다.  


Replit

![[p22-w04-4_screen_replit.png|500]]

리플릿.  
앞선 두 플랫폼보다는 퀄리티가 많이 떨어진다.  

그래도,  
직접 Gemini CLI 로 구현하고, 개선하는 시간에 비하면..

이렇게 되면, 먼저 바이브코딩 플랫폼에서 목업 이미지로 구현을 한 뒤에,  
수정을 하는 방식으로 해야하나 생각이 든다.  

---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p22-w04-4 - 메모앱 랜딩페이지 2번째](https://github.com/knachinen/one-day-one-project/tree/main/p22-w04-4_landing-memo-2) (github.com)
