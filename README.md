# AKLab
Android kernel exp lab is build for android kernel exploit practice, just for angler now.


## kernel info
based on android-msm-angler-3.10 (commit id:33ace82f84ba203ceb58b2c28a0f2e3389870030)

## vulnerbility 
* out of band write   -> build a vul device (path:/dev/vul)
* UAF  -> revert cve-2015-3636\<pingpongroot\> (as it is an 64bit version system, modify LIST_POISON2 from 0xdead000000000000 to 0x200200)
* racinng -> revert cve-2016-5195\<dirtycow\> 
* updating

## Test ENV
works fine with Android-8.1.0_r7 (BUILD_ID:OPM3.171019.013)

-------------------------------------------------------
## Get Image file from mega
[mega](https://mega.nz/#!SDo3DBgS!GtUqhU71mjqWg4POpHnxsrBgf_du4Cu5zilJ32DlMCw)

**(just for angler)**

1.It is a image.gz-dtb file,replace the image file in boot.img.

2.flash new boot.img file into your device,then it is a vul device.

3.Try exploit it.
