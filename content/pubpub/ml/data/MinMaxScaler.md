---
tags:
  - normalisation
  - sklearn
  - preprocessing
  - MinMaxScaler
---

```python
# Initialize MinMaxScaler with feature_range=(-1, 1)
scaler = MinMaxScaler(feature_range=(-1, 1))

# Fit and transform the data from df_a and df_b
rank_norm = scaler.fit_transform(df_merge_2024[['Rank_Diff']])
score_norm = scaler.fit_transform(df_merge_2024[['Score_Diff']])
```

