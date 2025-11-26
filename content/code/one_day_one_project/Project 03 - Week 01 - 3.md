---
id: "2025-1126_3-330-48_233053"
date: "2025-11-26"
time: "2025-11-26T23:30:53"
tags: 
status: 
category:
description: 
---

## 작업 요청

이번에는 AntiGravity 로 진행했다.  

`mvp 로서 아주 간단한 메모장`

몇 마디로 아주 간단하게 요청을 했는데,  
결과적으로 Gemini CLI 와는 다르게 알아서 잘 구현해줬다.  


## 구현 계획 

작업 요청에 따라 아래와 같은 계획을 작성해주었다.  

```markdown
## 목표 설명

React Native와 TypeScript 기반의 MVP 메모장 앱입니다. 기능: CRUD 작업, 로컬 저장소, 다크/라이트 모드, 프리미엄 글래스모피즘 디자인.

## 구현된 변경 사항

### 프로젝트 구조

디렉토리: `p03_w01-3_notepad`

#### App.tsx

- 메인 진입점.
- `notes` 상태 및 `themeMode` 상태 관리.
- 레이아웃 수정을 위한 `SafeAreaProvider` 처리.
- 테마 토글 구현 (☀️/🌙).

#### src/components/NoteList.tsx

- 메모 목록 표시.
- 적절한 패딩을 위해 `useSafeAreaInsets` 사용.
- 삭제 확인을 위한 `Alert.alert` 구현.
- 동적 스타일링을 위한 `theme` prop 수신.

#### src/components/NoteEditor.tsx

- 메모 작성 및 수정 인터페이스.
- 제목 자동 포커스.
- 동적 스타일링을 위한 `theme` prop 수신.

#### src/utils/storage.ts

- `saveNotes` / `loadNotes`: AsyncStorage에 메모 저장.
- `saveTheme` / `loadTheme`: 테마 설정 저장.

#### src/styles/theme.ts

- `ThemeColors` 인터페이스 정의.
- `THEMES` 내보내기 (다크/라이트).
- 동적 테마 생성을 위한 `createCommonStyles` 내보내기.

## 검증

- [ ]  Expo에서 앱 실행 (Android/iOS).
- [ ]  CRUD 작업 동작 확인.
- [ ]  재시작 후 데이터 유지 확인.
- [ ]  노치 디바이스에서 레이아웃 안전 확인.
- [ ]  삭제 확인 기능 동작 확인.
- [ ]  다크/라이트 모드 토글 및 유지 확인.
```

요청하지 않은 **글래스모피즘** 디자인까지 알아서 계획을 해주었다.  


## 결과 

대략 20분쯤 걸려서 코드 구현을 마쳤다.  
실행해보니 큰 오류 없이 잘 실행되었다.  

Gemini CLI 였다면 1시간 넘게 소요되었을 것이며,  
큰 오류도 여러군데에서 발생했을 것이다.  

자잘한 오류 몇 개와,  
안드로이드 상단바와 하단바와 겹치는 문제를 요청했고,  
금방 수정이 되었다.  

Gemini CLI 가 좀 더 손맛이 있긴 한데,  
앞으로는 시간상 반중력(AntiGravity)을 쓰는 게 좋을 것 같다.  


## 깃헙 레포 

> one-day-one-project/p03_w01-3_notepad at main · knachinen/one-day-one-project (github.com) | [Link](https://github.com/knachinen/one-day-one-project/tree/main/p03_w01-3_notepad) 


