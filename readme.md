
Building KryptonRom
--------------------


Initialize repo:

    repo init -u git://github.com/KryptonRom/manifest.git -b kitkat-remix
    
Sync the repo:

    repo sync
    
Build:

    . build/envsetup.sh && lunch

    make otapackage
    

Errors
-------
When met with sync error:

    check /.repo/local_manifests/roomservice.xml
    
Change errors to reflect correct repos , EG.

From
   
    <project name="AOSPA/AOSPA/android_device_lge_mako" path="device/lge/mako" remote="github" revision="kitkat" />
</manifest>
TO  
    <project name="AOSPA/android_device_lge_mako" path="device/lge/mako" remote="github" revision="kitkat" />
</manifest>
--------
