```
ffmpeg -r 15 -f image2 -i %06d.png -vcodec libx264 -crf 25 -pix_fmt yuv420p test.mp4
```
