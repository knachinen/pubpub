---
title: tqdm - total length
tags:
  - python
  - tqdm
  - darkmap
---

...

iteration 숫를 임의로 정할 때는 `total=` 매개변수를 쓰면 된다.

```python
total_length = len(filtered_df)
for index, row in tqdm(filtered_df.iterrows(), total=total_length):
    lat, long = sa.get_lat_long(row['지역'])
    filtered_df.at[index, '위도'] = lat
    filtered_df.at[index, '경도'] = long
```

...

## ref.

- 진행(progress)바/ tqdm :: 크레이지J의 탐구생활 (tistory.com) | [Link](https://crazyj.tistory.com/167) 


