---
title: "Beginner guide to install custom ROM on a Xiaomi phone"
date: 2020-09-29T19:34:03+05:30
draft: false
---

A custom ROM is one that has undergone any modification from being a pure distribution of Android. You can read more about it in detail in [this](https://www.androidauthority.com/what-is-a-custom-rom-android-74072/) article.

Steps to install a custom ROM:

1. Unlock Bootloader
2. Install custom Recovery
3. Flash ROM zip file
4. Flash root zip file
5. Reboot and enjoy!

---

## 1. Unlocking Bootloader

Different brands have their own individual methods of requesting permissions from the manufacturer to unlock bootloader. For Xiaomi phones, follow the following steps:

Step 1: Go to About Phone in Settings. Keep tapping `MIUI Version` until you get the message **You’re now a developer!** Now, go to Settings > Additional Settings > Developers Option and add you Mi account. Enable the `OEM Unlocking` & `USB Debugging` options.

Step 2: Download and extract [this](http://miuirom.xiaomi.com/rom/u1106245679/4.5.813.51/miflash_unlock-en-4.5.813.51.zip) zip to your Windows PC, run `miflash_unlock.exe` from the extracted folder and sign in with your Mi Account.

Step 3: Shut down your phone manually, then press and hold Volume down + Power button until your phone vibrates. This will take device into Fastboot mode.

Step 4. Connect your phone to PC using USB cable and click `Unlock`. Remember - **all your data will be deleted after this.** Your Bootloader will be unlocked after this.

---

## 2. Installing custom Recovery

Follow the following steps:

Step 1: Download and run [this](https://forum.xda-developers.com/attachment.php?attachmentid=4623157&d=1540039037) file. Write `Yes` when options are prompted.

Step 2: Download a Recovery image file for your device. I recommend [TWRP](https://twrp.me/Devices/Xiaomi/) Recovery. Click on `Primary (America)` link. Once downloaded, open the folder and rename it to _twrp-xxx.img_.

Step 3: Now, press Shift and Right Click on your mouse at any empty location in the folder. Select the option `Open Command Windows Here` and it will open the command prompt.

Step 4: Connect your device to PC via cable and type `adb reboot bootloader` in command prompt to boot your device into `Bootloader` mode. Click OK if asked for `Allow USB debugging` to continue.

Step 5: Come back to Command prompt & run `fastboot flash recovery twrp-xxx.img` and then `fastboot boot twrp-xxx.img` commands. Your device will boot into Recovery. Swipe right to _Allow modifications_, if prompted.

![TWRP Recovery](https://upload.wikimedia.org/wikipedia/commons/e/e0/TWRP_3.0.0-0.png)

---

## 3. Flashing ROM zip file

Step 1: Download a ROM file for your device. I recommend [Havoc OS](https://t.me/Havoc_OS). Download the _Gapps_ verison if you want to install a Pixel like OS in your phone.

Step 2: Go to `Wipe` then `Advanced Wipe`, select everything and swipe right to wipe.

Step 3: Connect device to PC again, and copy the downloaded zip file in your internal storage. If storage does not show up, go to `Mount` in TWRP and retick the internal storage option.

Step 4: Eject the device, Go to `Install` option and select the ZIP file. Check `Reboot after installation is complete.`

Congrats! Your device will boot into the freshly installed OS.

## 4. Flashing root zip file

Step 1: Download the [Magisk](https://github.com/topjohnwu/Magisk/releases/download/v20.4/Magisk-v20.4.zip) root zip.

Step 2: Press and hold all three buttons of your device until it vibrates and boot into the `TWRP recovery`.

Step 3: Install the `Magisk-vxx.x.zip` file similarly as you did the ROM file and reboot.

## 5. Enjoy your freedom!

If you run into any problems in the way, [ping](https://t.me/vvekm) me. Stay tuned for some more tutorials in future like installing YouTube premium for free on your rooted device.
