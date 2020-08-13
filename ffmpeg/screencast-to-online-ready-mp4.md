```
ffmpeg -f x11grab -r 60 -s 3840x2160 -i :0.0 -c:v qtrle screencast.mov 
```

```
for f in *.mov ; do
  bn=`basename $f .mov`
  ffmpeg -i $f -c:v libx264 -an -pix_fmt yuv420p $bn.mp4
done
```
