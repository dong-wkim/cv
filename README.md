---
title: bi-lingual CV/reśumé creation using multi-column markdown and pandoc
author: Dong Woon Kim
---

**Description**:
Creation of one dual-lingual document with side-by-side alignment from two separate markdown files, each written in a different language. Just write a document (such as a CV) in one language, then the same in another language, and this script will produce one document with both languages on one page.

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
