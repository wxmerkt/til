```bash
function favicon() {
  convert -resize x16 -gravity center -crop 16x16+0+0 -flatten -colors 256 $1 output-16x16.ico
  convert -resize x32 -gravity center -crop 32x32+0+0 -flatten -colors 256 $1 output-32x32.ico
  convert output-16x16.ico output-32x32.ico favicon.ico
  convert -resize x152 $1 apple-touch-icon-152x152.png
  convert -resize x120 $1 apple-touch-icon-120x120.png
  convert -resize x76  $1 apple-touch-icon-76x76.png
  convert -resize x60  $1 apple-touch-icon-60x60.png
  rm output-16x16.ico output-32x32.ico
}
```
