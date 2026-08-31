---
id: 2026-0831_1-243-36_222510
date: 2026-08-31
time: 2026-08-31T22:25:10
tags:
  - mosquito
  - detection
  - yolo
status:
category:
description:
---

.

모기 추적기를 만들고 있다.  

랩톱 카메라로 간단한 기초 파이프라인을 만든 뒤에,  
모기탐지 모델을 얹어서 실험해본 결과,  

![[annotated.gif]]

**...대실패!**  

![[compare_f2950.png|300]]

모기 4종을 학습한 모델로서 모기 이미지가 크고 확실한 형태는 탐지가 되는데,  
날파리처럼 보이는 이미지는 전혀 되지 않는다.  

게다가 엉뚱한 이미지를 인식한다.  

오픈소스로 공유된 모델이 잘 찾을 수 없어서,  
직접 모델을 만들어야 할 것 같다.  

- Model: 
	- iloncka/culico-net-det-v1: YOLOv11n fine-tuned on 4 species (Aedes aegypti, albopictus, Culiseta, japonicus-koreicus)
- Sample video:
	- Revenge on the mosquito that bit my daughter (with my mantis 'Kiwi') - YouTube (youtube.com) | [Link](https://www.youtube.com/watch?v=jbcwtDNQICg) 

