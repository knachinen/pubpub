---
title: pandas.concat
tags:
  - pandas
  - concat
  - darkmap
---

for loop 안에서 데이프레임 열을 추가하는 식으로 작성했는데,  
chatgpt 는 리스트를 만들고, 나중에 데이터프레임을 만드는 방식을 제안했다.  

이 때, `pandas.concat()` 함수를 사용한다.  
`pd.concat(df_a, df_b, columns=[,])` 형식으로 쓴다.  

```python
self.df_brief = pd.concat(
	[self.df_brief,
	 pd.DataFrame(
		 new_rows, 
		 columns=self.columns_brief)],
	ignore_index=True)
```