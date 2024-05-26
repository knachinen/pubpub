---
title: 
tags:
  - git
  - github
  - local
  - repository
  - connection
  - darkmap
---

할 때마다 깃헙 계정이 꼬여서, 이번 기회에 정리를 함.  

## process 


```bash
git init 
git config --local user.name "faf"
git config --local user.email "knachinen@gmail.com"
git add .
git commit -m "new: new files"
git remote add origin git@github.com:knachinen/darkmaptour_webscraping.git
git remote set-url origin git@github.com-knachinen:knachinen/darkmaptour_webscraping
git pull origin main
git push --set-upstream origin main
```


## ref.

- knachinen/darkmaptour_webscraping (github.com) | [Link](https://github.com/knachinen/darkmaptour_webscraping) | `w22.2024-05-26.Sunday, 23:04:45`
- [Git] 로컬 저장소(repository) 생성 후 원격 저장소(Github)와 연결 (tistory.com) | [Link](https://resultofeffort.tistory.com/99) | `w22.2024-05-26.Sunday, 23:08:15`
- 브랜치 생성과 삭제, 체크아웃 · Git, 분산버전 관리시스템 (gitbooks.io) | [Link](https://mylko72.gitbooks.io/git/content/branch/checkout.html) | `w22.2024-05-26.Sunday, 23:08:29`
