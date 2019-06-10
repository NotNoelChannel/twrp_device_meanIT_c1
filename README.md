# android_device_alps_z6u030
(aka GXQ6580 or gxq6580_weg_l)

Unofficial port of TWRP for a number of Mediatek MT6580-based Samsung Galaxy clones. Most of these devices receive little if any support due to their counterfeit nature, but some such as myself do work on these for the lulz since they're cheap and thus not as risky to mess around with.

* Compilation

        # repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-5.1
        
        # repo sync
        
        # . build/envsetup.sh

        # lunch omni_z6u030-eng

        # mka recoveryimage
        
If done correctly, you should end up with a recovery.img in `/out/product/alps/z6u030`.

You may also consult the TWRP guide at http://forum.xda-developers.com/showthread.php?t=1943625 in case you're stuck at any point during the build process.

## Issues/Caveats
* None so far.

## Downloads
You may download the recovery images for v105 and v107 here: https://github.com/huckleberrypie/android_device_alps_z6u030_twrp/releases
