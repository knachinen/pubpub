---
title: dataview - recently modified notes
tags:
  - dataview
  - obsidian
---

.

최근 썼던 노트들 목록이 필요했다.  
`cmd+o` 로 9개까지 볼 수 있기는 하지만,  
좀 더 많이 보고 싶었다.  

dataview 로 간단하게 목록을 만들 수 있다.  

```
TABLE dateformat(file.mtime, "yyyy-MM-dd,  HH:mm") AS "Last modified" 
FROM "" 
SORT file.mtime DESC 
LIMIT 25 
```

날짜 형식을 지정하고,  
정렬기준은 수정된 날짜기준 내림차순,  
목록 갯수는 25개.  


## ref.

- Dataview list of 25 most recently modified files in vault - Basement - Obsidian Forum (obsidian.md) | [Link](https://forum.obsidian.md/t/dataview-list-of-25-most-recently-modified-files-in-vault/23771) | `w23.2024-05-30.Thursday, 23:09:45`
- '옵시디언 활용/Dataview' 카테고리의 글 목록 (tistory.com) | [Link](https://kaminik.tistory.com/category/%EC%98%B5%EC%8B%9C%EB%94%94%EC%96%B8%20%ED%99%9C%EC%9A%A9/Dataview) | `w23.2024-05-30.Thursday, 23:10:09`


