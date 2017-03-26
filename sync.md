To get the resilio sync working, go to this site to install it:

https://help.getsync.com/hc/en-us/articles/206178924

Then request the key from Woody.


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

Look at the documentation for encf - there is a line to type in to de-encrypt.



