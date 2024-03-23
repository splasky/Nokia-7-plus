Nokia 7 plus bootloader unlock and tools
===

1. install drivers and adb drivers on windows
2. unlock the boot loader
follow the guide [[Guide] How to unlock the bootloader on Nokia Android Phones for free](https://www.techmesto.com/guide-unlock-bootloader-nokia-android-phones/), use the bootloader-unlock tool to unlock the bootloader
3. boot the device in fast-boot mode
```
adb reboot bootloader
```
4. boot the device in recovery mode
```
fastboot reboot recovery
```
5. boot to twrp recovery
```
sudo $(which fastboot) boot boot_b twrp.img
```
6. use twrp to or adb sideload to install new os
```
Select adb sideload
Type adb sideload rom-xyz.zip
adb reboot system
```