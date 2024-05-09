---
tags:
  - savefig
  - plot
---


```python
# save figure to image file
plt.savefig(
    'korea_press_freedom_index_score.png',
    dpi=200.0,
    bbox_extra_artists=(lgd,), 
    bbox_inches='tight'
)
```

