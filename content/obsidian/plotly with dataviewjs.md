



```dataviewjs 
let pages = dv.pages("#test/new");
//data:
//x: [0,1,2]
//y: [0,1,0.5]
dv.paragraph("```plotly"
    + `\ndata:\n- x: [0, 1, 2]\n`
    + `\n  y: [${pages.a.length}, ${pages.b.length}, ${pages.c.length}]\n`
    + "```"
)
```

