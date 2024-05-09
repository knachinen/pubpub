---
tags:
  - dataframe
  - plot
  - violinplot
  - fact-check
  - text
  - set_label_coords
---

바이올린 플롯 예시

```python
data = df_merge_2024['Score_Diff'].to_list()
data_sk = df_merge_2024[df_merge_2024['Country_EN'] == 'South Korea']['Score_Diff'].values[0]

plt.rcParams['font.family'] = 'SeoulNamsan'

ax = sns.violinplot(
    split=True, inner="quart", fill=False,
    data=data
)

# ax.yaxis.set_label_position("right")
ax.yaxis.tick_right()
ax.set_ylabel( 
    "언론 자유 지수 - 등락폭",
    # labelpad=20, rotation=90, 
    ha='right'
)
ax.yaxis.set_label_coords(1.15, 1)

plt.axhline(
    y=data_sk, 
    color='r', linestyle='-',
    linewidth=2,
    alpha=0.7
)

plt.text(
    x=0.5, y=data_sk, 
    s=f'{data_sk:.2f} 한국', 
    color='r',
    fontdict={
        'fontsize': 12,
        'fontweight': 'heavy'
    }
)

plt.xlabel('해당 점수의 국가분포')
plt.title('2024 언론 자유 지수 - 등락폭 비교')

plt.show()
```

![[pubpub/factcheck/rsf_2024_score_diff.png]]


