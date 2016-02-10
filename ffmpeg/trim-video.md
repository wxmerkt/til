# Trim Video

```
ffmpeg -ss 00:00:06 -i INPUT.mp4 -t 00:00:07 -c:v h264 OUTPUT.mp4
```

Where 6s is the starting time and 7s the duration.
