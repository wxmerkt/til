```sudo apt install v4l2-utils```

Set powerline frequency to 50 Hz:
```
v4l2-ctl -d /dev/video2 -c power_line_frequency=1
```

`/etc/udev/rules.d/81-uvcvideo.rules`:
```
# Set power line frequency to European
ACTION=="add", SUBSYSTEM=="video4linux", DRIVERS=="uvcvideo", RUN+="/usr/bin/v4l2-ctl --set-ctrl=power_line_frequency=1"
```
