```bash
for f in *.svg ; do
    base=`basename $f .svg`
    rsvg-convert -f pdf -o $base.pdf $f
done
```

## Installation
```bash
sudo apt-get install librsvg2-bin
```
