---
tags:
  - plot
  - font
  - line
  - annotate
  - min
  - max
  - savefig
  - fact-check
---

```python
plt.figure(figsize=(7, 3))
plt.rcParams['font.family'] = 'SeoulNamsan'

x_data = years[10:]
y_data = scores[10:]

sns.lineplot(x=x_data, y=y_data, marker='o', linestyle='-', color='green', linewidth=3)

max_score = max(y_data)
min_score = min(y_data)

# horizontal line
plt.axhline(y=max_score, color='blue', linestyle='-', label='역대 최고점수', linewidth=3, alpha=0.3)
plt.axhline(y=min_score, color='red', linestyle='-', label='역대 최저점수', linewidth=3, alpha=0.3)

# vertical line
plt.axvline(x='2013', color='orange', linestyle='--', label='이명박 - 박근혜', linewidth=3, alpha=0.5)
plt.axvline(x='2017', color='orange', linestyle='-', label='박근혜 - 문재인', linewidth=3, alpha=0.5)
plt.axvline(x='2022', color='brown', linestyle='-', label='문재인 - 윤석열', linewidth=3, alpha=0.5)

# Set x-axis and y-axis limits
plt.ylim([50, 100])

# Set y-axis limits
# plt.ylim([180, 1])

plt.yticks(np.arange(50, 100, 10))

# Annotate each point with its value
for year, score in zip(years, scores):
    if score == min_score:
        color = 'red'
        size = 16
        fontweight='heavy'
    elif score == max_score:
        color = 'blue'
        size = 16
        fontweight='heavy'
    elif year == '2024':
        color = 'brown'
        size = 16
        fontweight='heavy'
    else:
        color = 'grey'
        size = 12
        fontweight='normal'

    plt.annotate(
        f'{score}', (year, score), 
        textcoords="offset points", 
        xytext=(0,30), 
        arrowprops=dict(
            facecolor=color,
            arrowstyle=ArrowStyle('simple', head_length=0.4, head_width=0.4, tail_width=0.2),
            alpha=0.5
        ),
        ha='center', 
        color=color,
        size=size,
        fontweight=fontweight
    )
    
# Add labels to the axes and a title to the plot
plt.xlabel('년도', labelpad=15)
plt.ylabel('언론 자유 지수 - 점수')
plt.title('국경없는기자회 2013-2024 대한민국 언론자유지수 - 점수 변화')
lgd = plt.legend(loc='center left', bbox_to_anchor=(1, 0.5))

# save figure to image file
plt.savefig(
    'korea_press_freedom_index_score.png',
    dpi=200.0,
    bbox_extra_artists=(lgd,), 
    bbox_inches='tight'
)

# Show the plot
plt.show()
```

![[pubpub/factcheck/rsf_sk_score.png]]
