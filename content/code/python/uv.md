---
title: uv
tags:
  - uv
  - python
  - devops
description: 
aliases: 
date: 2025-07-21T23:22:58
---

.

pyenv + poetry 를 줄곧 써왔는데,  
가끔씩 파이썬 가상환경이 제대로 안 돌아갈 때가 있었다.  
너무 많은 환경이 꼬여있어서 왜 그런지 잘 모르겠다.  
이참에 uv 를 써보기로 했다.  

uv 는 다른 프로젝트에서 쓴다고 이미 있어서,  
업데이트하고 초기화만 하고 쓸 수 있었다.  

```bash
uv self update
uv init web-preview
uv venv
source .venv/bin/activate
uv add jupyter ipywidgets
```

가상환경 활성화도 잘되고,  
패키지 설치도 빨라 보인다.  

## ref. 


- GitHub - astral-sh/uv: An extremely fast Python package and project manager, written in Rust. (github.com) | [Link](https://github.com/astral-sh/uv) 
- Installing and managing Python (uv) | [Link](https://docs.astral.sh/uv/guides/install-python/) 
- python의 uv 사용법 - [루닥스 블로그] 연습만이 살길이다 (tistory.com) | [Link](https://rudaks.tistory.com/entry/python%EC%9D%98-uv-%EC%82%AC%EC%9A%A9%EB%B2%95) 
- 파이썬 개발자라면 uv 를 사용합시다. Poetry, Anaconda, virtualenv 는 이제 그만! | by Sigrid Jin (Medium) | [Link](https://sigridjin.medium.com/%ED%8C%8C%EC%9D%B4%EC%8D%AC-%EA%B0%9C%EB%B0%9C%EC%9E%90%EB%9D%BC%EB%A9%B4-uv-%EB%A5%BC-%EC%82%AC%EC%9A%A9%ED%95%A9%EC%8B%9C%EB%8B%A4-546d523f7178) 

.

