# Screenshot/Screen Capture from video

```
ffmpeg -ss 01:23:45 -i input -vframes 1 -q:v 2 output.jpg
```

Source: http://stackoverflow.com/a/27573049

# Video to frames

```
ffmpeg -i input.mp4 -r 30 -quality 100 frames_%04d.jpg
```
