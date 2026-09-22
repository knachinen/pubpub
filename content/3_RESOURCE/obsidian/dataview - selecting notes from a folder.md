---
title: dataview - selecting notes from a folder
tags:
  - obsidian
  - dataview
  - folder
description: get list of notes from a specific folder with dataview
aliases: 
date: 2024-06-10
---

.

특정 폴더 안에 있는 노트들의 목록을 뽑아내고 싶었는데,  
contains() 를 쓰면 된다.  

```
LIST WHERE contains(file.folder, this.file.folder)
SORT file.ctime DESC
```

## ref. 


- Listing all files within a directory that the current note is in - current folder - Basement - Obsidian Forum (obsidian.md) | [Link](https://forum.obsidian.md/t/listing-all-files-within-a-directory-that-the-current-note-is-in-current-folder/20869/4) 

