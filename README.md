---
title: bi-lingual CV/reśumé creation using multi-column markdown and pandoc
author: Dong Woon Kim
---

**Description**:
Create a CV in two languages, side-by-side in two columns using markdown and pandoc.

**Step 1**: install pandoc

```
sudo apt install pandoc
```

**Step 2**: download columns.lua from github.com/pandoc/filters/columns/columns.lua.

```
git clone https://github.com/pandoc/filters/columns/columns.lua <pandoc directory>

```

And place columns.lua into directory with cv.md file. Open terminal in directory with cv.md and cv.md.


**Step 3**: create PDF version by invoke pandoc with lua filter extension

```
pandoc --lua-filter="columns.lua" -o cv.pdf cv.md
```
