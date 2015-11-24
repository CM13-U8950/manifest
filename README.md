slim6.0_manifest
================

Local Manifest to build Slim6.0 for the Huawei U8950 (Honor Pro)

Build Instructions
-----------------------------------------------------------------------------

1. Initialize repo using the Slim6.0 manifest
    
        repo init -u git://github.com/SlimRoms/platform_manifest.git -b mm6.0

2. Add my local manifest

        curl --create-dirs -L -o .repo/local_manifests/slim_huawei.xml -O -L https://raw.github.com/SlimM-U8950/manifest/mm6.0/slim_huawei.xml

3. Then sync up the repositories
 
        repo sync

4. Build the ROM

        brunch u8950

