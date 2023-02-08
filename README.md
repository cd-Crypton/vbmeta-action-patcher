## Patch your VBMeta Image
This github action will let you patch your vbmeta. Prebuilt files for patching aren't mine, all the credits should be given to him; [lbxzr](https://github.com/libxzr)'s [vbmeta-disable-verification](https://github.com/libxzr/vbmeta-disable-verification).

## Guide
* Fork this repository.
* Replace `vbmeta.img` with your stock or from android (google) source.
* Go to `Action` tab, then Run the workflows.
* Go to `Release` section of the repository, download the new vbmeta image, and flash it.

## Notes
* It is equivalent to: `fastboot --disable-verity --disable-verification flash vbmeta vbmeta.img`.
* If patching failed, maybe you are patching using wrong architecture;
  * Check Operating System Information in the workflow results.
  * If your Operating System Information tells you x86_64, then you need to use x86_64 as architecture.
