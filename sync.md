
## Get on the network

Log onto the wifi

## Get CHC files synced

Request the key from IT officer or someone else on the network.

### Windows and Mac

Install resilio and follow instraction

### Ubuntu

To get the resilio sync working, go to this site to install it:

https://help.getsync.com/hc/en-us/articles/206178924

```
sudo systemctl enable resilio-sync
systemctl --user start  resilio-sync
```

Then navigate to here:

http://localhost:8888/gui/

Click on the down arrow and click 'enter key'.

To de-encrypt, install encf:

```
sudo apt install encfs  
```

Look at the documentation for encf - there is a line to type in to de-encrypt - see here:

https://www.howtoforge.com/tutorial/encrypt-your-data-with-encfs-on-ubuntu/

To sync the folder, type:

```
encfs ~/Resilio\ Sync/Cornerstone/ ~/cornerstone 
```

To unmount the volume in this case, you would [enter](https://www.howtoforge.com/tutorial/encrypt-your-data-with-encfs-debian-jessie/):

```
fusermount -u ~/cornerstone
```


