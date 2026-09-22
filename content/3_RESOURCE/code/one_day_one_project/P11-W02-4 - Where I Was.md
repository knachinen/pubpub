---
id: "2025-1204_4-338-49_184549"
date: "2025-12-04"
time: "2025-12-04T18:45:49"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] Where I Was (어디갔었지?)
> - 갔던 장소 아카이브. 

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
> - Feasibility 와 PRD 문서를 바탕으로 계획과 작업 목록 작성.

문서만 작성하라고 안해서 그런지, 바로 구현을 시작해버림.  

---

## 작업 문서 

> [!EXAMPLE] 문서
> - 실현가능성 검토 : [Feasibility](https://github.com/knachinen/one-day-one-project/blob/main/p11_w02-4_where-i-was/doc/p11_w02-4_feasibility.md)
> - 제품명세서 : [PRD](https://github.com/knachinen/one-day-one-project/blob/main/p11_w02-4_where-i-was/doc/p11_w02-4_where-i-was.md)
> - 구현 계획 : [Implementation Plan](https://github.com/knachinen/one-day-one-project/blob/main/p11_w02-4_where-i-was/doc/implementation_plan.md)
> - 작업 목록 : [Task](https://github.com/knachinen/one-day-one-project/blob/main/p11_w02-4_where-i-was/doc/task.md)
> - 기술 검토 : [Walkthrough](https://github.com/knachinen/one-day-one-project/blob/main/p11_w02-4_where-i-was/doc/walkthrough.md)

---

## 개발 과정 

디버깅으로 앱이 무난하게 작동하는 정도가 되었고,  
나름 쓸만해보여서 아이콘을 생성요청하여 적용하였다.  

### 앱 아이콘과 스플래시 아이콘 생성

![[p11-w02-4_icon.png]]

![[p11-w02-4_splash.png]]

---
## 디버깅 및 결과 

![[p11-w02-4_screen.png]]

구현 뒤에 앱 충돌문제로 꺼지는 문제가 있었다.  
로깅하고, 로그를 트래킹해서 수정하는데 그렇게 오래 걸리지는 않았다.  

원래 계획은 백그라운드로 실행이 되면서 자동으로 위치를 트래킹하고, 저장하도록 만들어졌다.  
사용하는데 오히려 불편할 것 같아서, 수동 위치 저장하도록 변경했다.  


> [!SUCCESS] 디버깅 후 고쳐진 오류들
> - 구현 뒤 앱 실행하면 충돌로 종료됨 
> - 구글맵에서 오픈스트릿맵 사용
> - 백그라운드 기능 취소, 수동 위치 저장
> - 현재위치, 저장된 위치 표시
> - 마커 적용
> - 다른 위치 저장
> - 외부 데이터 불러올 때 중복처리
> - 레거시 아키텍처를 쓰고있다고 새로운 아키텍터를 쓰라고 경고. 
> - 아이콘이 적용안됨. 


> [!BUG] 수정되지 않은 오류들
> - 대부분의 버그는 수정됨
> - 내비게이션바 투명도



---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [P11-W02-4 - Where I Was](https://github.com/knachinen/one-day-one-project/tree/main/p11_w02-4_where-i-was/) (github.com)
