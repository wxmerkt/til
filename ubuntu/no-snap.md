Cf. https://askubuntu.com/a/1285102:
```bash
# stop snapd services
sudo systemctl stop snapd && sudo systemctl disable snapd
# purge snapd
sudo apt purge snapd
# remove no longer needed folders
rm -rf ~/snap
sudo rm -rf /snap /var/snap /var/lib/snapd /var/cache/snapd /usr/lib/snapd
```
