1. ```sudo apt install libimobiledevice6 libimobiledevice-utils ifuse```
2. ```idevicepair pair```
3. ```usbmuxd -f -v```
4. get the UUID with: `lsusb -v 2> /dev/null | grep -e "Apple Inc" -A 2`
5. open the phone with `afc://UUID:1`

