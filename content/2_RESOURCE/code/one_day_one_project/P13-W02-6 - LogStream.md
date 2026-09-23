---
id: "2025-1206_6-340-49_104518"
date: "2025-12-06"
time: "2025-12-06T10:45:18"
tags: 
status: 
category:
description: 
---
## 프로젝트 아이템

> [!INFO] 디바이스 로그 확인
> - 안드로이드 디바이스 시스템 로그를 보여주는 앱

---

## 개발환경

> [!INFO] IDE & 모델
> - IDE: 반중력편집기 (AntiGravity)
> - 모델
> 	- 계획: Claude Sonnet 4.5
> 	- 구현: Gemini 3 Pro (High)
> 	- 디버깅: Gemini 3 Pro (High)

  

---

## 작업 요청

### 실현 가능성 검토 (Gemini Web)

> [!QUESTION] Gemini 프롬프트
> - 안드로이드 시스템 로그 기록을 확인할 수 있는 앱
> 	- 실현 가능성
> 	- 구현 가능한 기능
> 	- 난이도
> - 프로젝트 : 안드로이드 로그 뷰어. 라텍스 문법 제외.
> 	- (실현 가능성 답변 첨부)


### 목업 디자인 (Stitch)


> [!QUESTION] Stitch 프롬프트
> - PRD 바탕으로 앱 디자인
> 	- (PRD 답변 첨부)


![[p13-w02-6_mockup.png]]


### 작업 요청 (반중력)

> [!QUESTION] 반중력 프롬프트
> - 🔍  제품 요구사항 명세서를 개선점을 파악하고, 수정 보완하기. 문서만 업데이트하고 지시 기다릴것.
> - 📱  목업 디자인 요구사항 정리
> - 📋  구현 계획, 구현 작업 목록 작성 
> - ▶️  문서 작성 후 구현 자동 시작


---

## 작업 문서 

> [!EXAMPLE] 문서
> - 실현가능성 검토 : [Feasibility](https://github.com/knachinen/one-day-one-project/blob/main/p13_w02-6_logstream/doc/feasibility.md)
> - 제품명세서 : [PRD](https://github.com/knachinen/one-day-one-project/blob/main/p13_w02-6_logstream/doc/prd.md)
> - 디자인 : [Design](https://github.com/knachinen/one-day-one-project/blob/main/p13_w02-6_logstream/doc/design.md)
> - 구현 계획 : [Implementation Plan](https://github.com/knachinen/one-day-one-project/blob/main/p13_w02-6_logstream/doc/implementation_plan.md)
> - 작업 목록 : [Task](https://github.com/knachinen/one-day-one-project/blob/main/p13_w02-6_logstream/doc/task.md)
> - 기술 검토 : [Walkthrough](https://github.com/knachinen/one-day-one-project/blob/main/p13_w02-6_logstream/doc/walkthrough.md)

---

## 개발 과정 

### 구현 후 첫 실행


> [!BUG] 
> - The development server returned response error code: 500

```bash
Unable to resolve "react-native-gesture-handler" from "App.tsx"
> 1 | import 'react-native-gesture-handler';
    |         ^
  2 | import React from 'react';
  3 | import { AppNavigator } from './src/navigation/AppNavigator';
  4 | import { useLogStream } from './src/hooks/useLogStream';

Import stack:

 App.tsx
 | import "react-native-gesture-handler"

 index.ts
 | import "./App"
 | import "./index"

```

```bash
npm install react-native-gesture-handler @react-native-community/masked-view react-native-reanimated 
npx expo install --fix 
```

### 구현 기능 검증

> [!BUG] 
> - Saving logs

```bash
 WARN  Method readDirectoryAsync imported from "expo-file-system" is deprecated.
 ERROR  [Error: Method readDirectoryAsync imported from "expo-file-system" is deprecated.
 WARN  Method writeAsStringAsync imported from "expo-file-system" is deprecated.
```

```
 ERROR  [Error: Method getInfoAsync imported from "expo-file-system" is deprecated.
 ERROR  Failed to save logs: [TypeError: logFile.exists is not a function (it is false)]

```

### 수정 보완

> [!BUG] 
> - UI 색상 
> - 멈춤 버튼이 잘 동작하지 않음. 
> 	- 디바이스 성능이 로깅을 처리하기에 너무 느린가? 
> - 최신 로그 스크롤 
> - 로그 업데이트 속도

---
## 결과 

![[p13-w02-6_screen.png]]

> [!SUCCESS] 최종 기능 구현
> - 로그뷰 
> - 로그 시작/멈춤/초기화
> - 로그 저장
> - 로그 키워드 검색
> - 아래 스크롤 



---
## 깃헙 레포 

> [!INFO] 깃헙 레포지토리
> [p13_w02-6_LogStream](https://github.com/knachinen/one-day-one-project/tree/main/p13_w02-6_logstream) (github.com)
