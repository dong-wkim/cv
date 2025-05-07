# CV/Reśumé

Create a CV in two languages, side-by-side in two columns using markdown and pandoc.

**Step 1**: install pandoc

```
sudo apt install pandoc
```

**Step 2**: download columns.lua from github.com/pandoc/filters/columns/columns.lua.

```
git clone https://github.com/pandoc/filters/columns/columns.lua <pandoc directory>

```

**Step 3**: create PDF version by invoke pandoc with lua filter extension

```
pandoc --lua-filter="/Users/dongwkim/.pandoc/filters/columns.lua" -o cv.pdf cv.md
cv.pdf
```
