# android_device_alps_z6u030
(aka GXQ6580 or gxq6580_weg_l)

Unofficial port of TWRP for a number of Mediatek MT6580-based Samsung Galaxy clones. Most of these devices receive little if any support due to their counterfeit nature, but some such as myself do work on these for the lulz since they're cheap and thus not as risky to mess around with.

To build from source, clone this repo or download this branch as a ZIP, then follow the TWRP guide at http://forum.xda-developers.com/showthread.php?t=1943625

Copy the contents of this repo in `/your_source_folder_here/device/alps/z6u030`, key in `source ./build/envsetup.sh`, then `lunch`, select `omni_z6u030-eng` then `make clean && make -j# recoveryimage`, replacing `-j#` with either `j3` or `j5` depending on your processor. On a dual core, you should use `j3`.

If all goes well, you should end up with a freshly-cooked recovery.img in `/out/product/z6u030`.

## Issues/Caveats
* Recent versions of SuperSU may fail to install with a "BAD RECOVERY DETECTED" error, c.f. https://github.com/TeamWin/Team-Win-Recovery-Project/issues/367 - not much I could do so far with that one; I did however include a SuperSU installer in the image as a workaround. Alternatively you may try phh's Superuser utility, owing to issues with SuperSU being closed-source and all...

## Downloads
You may download the initial recovery releases for v105 and v107 here: https://github.com/huckleberrypie/android_device_alps_z6u030/releases
