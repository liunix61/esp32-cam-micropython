
Please go to the new repository https://github.com/shariltumin/esp32-cam-micropython-2022

# esp32-cam-micropython

**Latest** custommade.zip, please read [this blog](https://kopimojo.blogspot.com/2019/12/custom-made-sometimes-it-is-nice-to-be.html) and find out what it is good for.

The custommade.zip now contains files that will also include LittleFS in the firmware for esp32-cam, esp32 and esp8266. Please watch Damien George explaining what LittleFS is good for, at a [Melbourne micropython meeting](https://www.youtube.com/watch?v=wkgU4fGP3eY). 

You can use LittleFS instead of FatFS(default) by doing these in REPL:

```
>>> import os
>>> os.VfsLfs2.mkfs(bdev)

```

You will save RAM if you use LittleFS. The FS setting will survive reboot and power cycle.


The files in the directories under are obsolete:

1. esp32-cam-1-11-498
2. esp32-cam-1-11-571


Please use files under Custommade_Template directory packed in the custommade.zip. Better yet run mpb.py to build custom made firmware.

If you're looking for a compiled firmware that support camera for your esp32-cam board then please click [firmwares](https://github.com/shariltumin/esp32-cam-micropython/tree/master/firmwares).

You can find some webcam server test scripts in [webcam](https://github.com/shariltumin/esp32-cam-micropython/tree/master/webcam). **Latest** is [mth_webcam.py](https://github.com/shariltumin/esp32-cam-micropython/blob/master/webcam/mth_webcam.py) a multi-threaded three ports web server. Serving webcam at port 80.

I record my works at [kopimojo.blogspot.com](https://kopimojo.blogspot.com/) feel free to drop by.
