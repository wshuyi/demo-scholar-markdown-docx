基础使用
```bash
pandoc demo.md -o demo.docx
```

带latex公式
```bash
pandoc demo-math.md -o demo-math.docx
```

带脚注
```bash
pandoc demo-footnote.md -o demo-footnote.docx
```

带引用
```bash
# 旧版 pandoc --filter pandoc-citeproc --bibliography=myref.bib --csl=chinese-gb7714-2005-numeric.csl demo-citation.md -o demo-citation.docx

pandoc --citeproc --bibliography=myref.bib --csl=chinese-gb7714-2005-numeric.csl demo-citation.md -o demo-citation.docx
```

带图片引用
```bash
# 旧版pandoc --filter pandoc-fignos --filter pandoc-citeproc --bibliography=myref.bib --csl=chinese-gb7714-2005-numeric.csl demo-figref.md -o demo-figref.docx

pandoc --filter pandoc-fignos --citeproc --bibliography=myref.bib --csl=chinese-gb7714-2005-numeric.csl demo-figref.md -o demo-figref.docx
```
