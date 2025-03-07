# cv/resume

## Step 1: Save columns.lua into pandoc/filters directory and cd into the directory with the cv.md markdown file

```
cd obsidian

```

## invoke pandoc with lua filter

```
pandoc --lua-filter="/Users/dongwkim/.pandoc/filters/columns.lua" -o cv.pdf curriculum_vitae.md
cv.pdf
```
