# Essentialphone-root
## a record of how to root essential phone
Essential phone is designed with a/b slots

Step 1: install essential phone driver from this official [link](https://essentialsupport1493251565.zendesk.com/hc/en-us/articles/115015490828-Windows-Drivers-for-Essential-Phone)

Step 2: reboot the phone into fastboot mode
```
adb reboot bootloader
```


Step 3: find current slot
```
fastboot getvar current-slot
```
and change to the other slot
```
fastboot -aX
```
X is a or b

Step 4: flash the TWRP-SEP image (note that other images are not functionable to touch)
```
fastboot flash boot TWRP-SEP.img
```
