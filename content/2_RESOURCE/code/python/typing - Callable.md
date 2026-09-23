---
title: typing - Callable
tags:
  - python
  - typing
  - callable
  - darkmap
---

...

함수의 매개변수 타입을 정의하는데,  
함수형일 때에는 어떻게 하지?   

```python
type(scr.get_article_text)
```

```
method
```

타입이 메서드로 나오길래 해봤더니, 그런 타입은 없다며 에러가 난다.  

...

함수형일 때에는 다음과 같이,  
typing 의 Callable 로 정의를 한다.  

```python
from typing import Callable


    def get_article_text(
        self,
        html:str,
        get_text_html_func: Callable[[BeautifulSoup], str]
    ) -> str:
        soup = BeautifulSoup(html, 'html.parser')
        text = get_text_html_func(soup)


def get_text_hk(soup: BeautifulSoup) -> str:
    article_body = soup.find_all("div", class_="article-body")
    if len(article_body) != 0:
        return article_body[0].get_text()
    else:
        return ""

```


