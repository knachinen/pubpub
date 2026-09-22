---
title: templater
tags:
  - obsidian
  - plugin
  - templater
description: obsidian plugin templater
aliases: 
date: 2024-06-10 22:55
---

.

옵시디언의 unique note creator 와 templates 를 쓰고 있었는데,  
templater 플러그인을 한번 써보고 싶었다.  

templater 에서는 `{{}}` 태그 대신에 `<% tp.xxx %>` 를 쓴다.  

```markdown
---
title: <% tp.file.title %>
tags:
description: 
aliases: 
date: <% tp.file.creation_date() %>
---

.



## ref. 

- 
```


## error

하지만 못 쓰게 되었다.  
quartz 에서는 `%` 를 쓰면 안되는 것 같다.   

```bash
Failed to process `content/obsidian/templates/content.md`: bad indentation of a mapping entry (2:8)

  1 |
  2 | title: %
 ------------^
  3 | tags:
  4 |   - obsidian
     at Object.yaml [as parse] (../plugins/transformers/frontmatter.ts:55:35)

```

그냥 옵시디언 기본 templates 를 쓰고,  
다른 볼트에서 써야겠다.  


## ref. 

- Obsidian 옵시디언, Templater 플러그인 (tistory.com) | [Link](https://olait.tistory.com/14) 
- Introduction - Templater (github.io) | [Link](https://silentvoid13.github.io/Templater/) 

.

