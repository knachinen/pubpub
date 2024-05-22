---
title: findall, search, sub
tags:
  - regular-expression
  - darkmap
---

- `findall()` : 텍스트에서 패턴과 일치하는 모두를 찾음

```python
import re

text = "Hello, world! Hello, universe!"
matches = re.findall(r'Hello', text)
print("Matches found:", matches)
```

```
Matches found: ['Hello', 'Hello']
```

- `search()` :  일치하는 패턴 하나를 찾음. 첫번째 찾은 패턴.

```python
import re

text = "Hello, world!"
match = re.search(r'world', text)
if match:
    print("Found:", match.group())
else:
    print("Not found")
```

```
Found: world
```

- `sub()` :  패턴을 찾아 원하는 텍스트로 바꿈


## 다크맵에 쓰인 코드

```python
def re_pattern(keyword: str) -> str:
    # Define the pattern to search for the keyword, with word boundaries to match whole words only
    return r'\b{}'.format(re.escape(keyword))


def re_findall(keyword: str, text: str) -> str:
    # Find all matches of the pattern in the text (case-insensitive)
    return re.findall(re_pattern(keyword), text, flags=re.IGNORECASE)


def re_search(keyword: str, text: str) -> str:
	# Searches for the given keyword in the text using a regular expression.
    return re.search(r'\b{}'.format(keyword), text, re.IGNORECASE)


def re_sub(keyword: str, text: str) -> str:
    # Use re.sub to replace the keyword with the keyword surrounded by parentheses
    return re.sub(re_pattern(keyword), r'🔺\g<0>🔻', text, flags=re.IGNORECASE)

```

