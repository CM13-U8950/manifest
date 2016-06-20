cm13.0_RR_manifest
================

Local Manifest to build CM13 and ResurrectionRemix for the Huawei U8950 (Honor Pro)

Build Instructions
-----------------------------------------------------------------------------

1. Initialize repo using the CM13 manifest
    
        repo init -u git://github.com/CyanogenMod/android.git -b cm-13.0

   Or Initialize repo using the ResurrectionRemixM manifest
        
        repo init -u git://github.com/ResurrectionRemix/platform_manifest.git -b marshmallow

2. Add my local manifest

        curl --create-dirs -L -o .repo/local_manifests/cm_huawei.xml -O -L https://raw.github.com/CM13-U8950/manifest/cm-13.0/cm_huawei.xml

3. Then sync up the repositories
 
        repo sync -f

4. Build the ROM

        . build/envsetup.sh

        brunch u8950

