```dataviewjs
dv.table(["Status","Title", "Author", "Progress"], 
    dv.pages('#📚Book')
      .filter(p => !p.file.path.includes("Templates"))
      .map(p => [
	      p.status,
          p.file.link, 
          p.author, 
          dv.span(
              `![progress](https://progress-bar.xyz/${parseInt((p.currentPages / p.totalPages) * 100)}/)`
          )
      ])
);
```
