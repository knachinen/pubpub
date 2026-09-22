---
title: dataframe.sort_values
tags:
  - pandas
  - sort
  - darkmap
---

```python 
df_brief.sort_values(by=['level'], axis=0, ascending=False)
```

|     | original_name | found_name | level | count | upper |
| --- | ------------- | ---------- | ----- | ----- | ----- |
| 1   | 태안읍           | 태안읍        | 3     | 2     | 태안    |
| 0   | 태안군           | 태안         | 2     | 2     |       |
| 3   | 화성시           | 화성         | 2     | 6     | 경기    |
| 2   | 경기            | 경기         | 0     | 1     |       |

## ref.

- R, Python 분석과 프로그래밍의 친구 (by R Friend) :: [Python] 데이터 정렬 (sort, arrange) : DataFrame.sort_values(), sorted(), list.sort() (tistory.com) | [Link](https://rfriend.tistory.com/281) 