cm13.0_manifest
================

Local Manifest to build CM13 for the Huawei U8950 (Honor Pro)

Build Instructions
-----------------------------------------------------------------------------

1. Initialize repo using the CM13 manifest
    
        repo init -u git://github.com/CyanogenMod/android.git -b cm-13.0

2. Add my local manifest

        curl --create-dirs -L -o .repo/local_manifests/cm_huawei.xml -O -L https://raw.github.com/CM13-U8950/manifest/cm-13.0/cm_huawei.xml

3. Then sync up the repositories
 
        repo sync

4. Build the ROM

        brunch u8950

