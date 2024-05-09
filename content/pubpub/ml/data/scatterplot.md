---
tags:
  - scatterplot
---

```python
ax2 = sns.scatterplot(
    data=df_merge_2024, 
    x="Rank_Diff_Reversed",
    y="Score_Diff"
)
ax2.yaxis.set_major_formatter('{x:+}')
ax2.xaxis.set_major_formatter('{x:+}')

for x, y, label, tag in annotations:

    if tag == 'red':
        color = 'red'
        text = label
        xypoint = (x, y)
        xytext = (-30, 50)
        fontsize = 14
    elif tag == 'lower':
        color = 'grey'
        text = label
        xypoint = (x, y)
        xytext = (30, -50)        
        fontsize = 8
    else:
        color = 'grey'
        text = label
        xypoint = (x, y)
        xytext = (-30, 50)
        fontsize = 8

    arrowstyle = ArrowStyle('simple', head_length=0.5, head_width=0.5, tail_width=0.2)

    arrowprops = dict(
        facecolor=color,
        arrowstyle=arrowstyle,
        alpha=0.5
    )

    ax2.annotate(
        text, xypoint, 
        textcoords="offset points", 
        xytext=xytext, 
        arrowprops=arrowprops,
        ha='center', 
        color=color,
        size=fontsize,
        fontweight='heavy',
        alpha=0.7
    )
    
plt.show()
```

![[pubpub/ml/data/scatterplot_sk_others.png]]

