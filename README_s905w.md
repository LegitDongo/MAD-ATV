For the X96 mini 2gb/16gb (s905w) and the a95x f1
<br>(and probably some other s905w boxes)
<br>
<br>INSTALLATION:
<br>
<br>After you flashed the rom:
<br>* Let the system fully boot.
<br>* Fill in the setup menu fast if you can, once the box has internet it will download and install the latest pogodroid and RGC.
<br>* After it finishes this it will boot in to TWRP. In TWRP slide to allow system mods, then choose install and select Magisk-v18.1.zip, then add more zips and select smali.zip.
<br>* Install the zips and then wipe cache/dalvik cache. Reboot the system and let Android load.
<br>* Go to Android settings, about, scroll down and click build until it says you are a developer. Then go to Android settings - developer settings - turn on "stay awake"
<br>* Now go to magisk and double check that you pass safetynet.
<br>* In magisk settings repackage magisk.
<br>* Now go to pokemon go and sign in. You will need to use scrcpy or teamviewer to enter data in to the pokemon go app.
<br>* Configure RGC and Pogodroid (I give them 10 seconds delay to start and I leave pogodroid at 120 seconds before injection.
<br>
<br>You will need to use scrcpy or something similar (teamviewer or whatever?) in order to interact with pokemon go. To use scrcpy in portrait mode, be sure you use the adb.exe which is in the scrcpy dir, and then start scrcpy from cmd via scrcpy.exe -b2M -m1024 (many people have sent many suggestions for settings for this command, feel free to set bitrate and res to whatever makes you happy :) )
<br>
<br>[This recovery](https://github.com/Map-A-Droid/MAD-ATV/raw/master/recovery_rare_x96.img) was needed by 2 x96 mini users. They installed the MAD rom and then when it rebooted to recovery nothing loaded. They also could not load the recovery manually by pressing the button inside the AV port while giving it power. This recovery worked for both of them. To use it, format a sd card with fat16 or fat32 and put this file on it named recovery.img and then insert the card into the box without power. While pressing the reset button plug in the power cable and hold down the reset button until the recovery loads. Then continue with Magisk installation.