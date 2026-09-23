---
title: autoreload
tags:
  - python
  - autoreload
  - package
  - jupyter-notebook
---

...

jupyter notebook 에서 임포팅한 모듈을 쓰는데,  
모듈을 수정을 할 때마다 리프레시를 해주는 게 정말 번거롭다.  

그리하여 알게 된 `autoreload` 
셀을 실행할 때마다 해당 모듈을 다시 임포팅한다.  

## src.

```python
%load_ext autoreload
%aimport utils.webscraping

from utils.webscraping import ArticleScraper, get_text_hk

%autoreload 2
```



## ref. 

- autoreload — IPython 8.24.0 documentation (readthedocs.io) | [Link](https://ipython.readthedocs.io/en/stable/config/extensions/autoreload.html) | `w23.2024-05-28.Tuesday, 23:46:36`