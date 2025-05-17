<div align="center">

  # Camaleon
  ### A theme engine to camouflage the user interface on Android 12+ devices.
🎨 Camaleon theme engine is a collection of the [Iris](https://play.google.com/store/apps/details?id=arz.substratum.iris.monet) and [Eclipse](https://play.google.com/store/apps/details?id=arz.substratum.eclipse) substratum themes, with enhancements that allows you to easily customize the style of the user interface, such as icons, colors and more, even for some third-party apps.

</div>

# ⚙️ REQUIREMENTS
- Pixel or AOSP based custom ROM.
- ROOT access ([Magisk](https://github.com/topjohnwu/Magisk) (Recommended) / [KernelSU](https://github.com/tiann/KernelSU) / [APatch](https://github.com/bmax121/APatch)).
- [Unlocker](https://play.google.com/store/apps/details?id=com.arz.camaleon.unlocker) app (paid) to access premium features (optional).
- Custom recovery supported by decryption, ROM compatible with safe mode boot or PC (just in case there is a possible bsod/bootloop).

# 🔧 How to install?
- Install the unlocker app and Camaleon.
- Open Camaleon and grant permissions.
- Tap the install button and wait for the app to finish.
- Reboot and enjoy!
> KernelSU users need to manually allow root access for Camaleon from the 
 KernelSU app itself.

# 💿 Compatibility
- ✅ Supported Android 12-15.
- ❌ OEM systems such OxygenOS, MIUI, OneUI, etc. are not supported.

# 🖊️ Notes
- <b>Do not enable QS styles others than "Universal"</b> variant on DerpFest Android 12L.

# 🛟 In case of bsod/bootloop
- The best solution is to start in safe mode, or delete the <b>'Camaleon'</b> folder from <b>'/data/adb/modules/'</b> if you have a custom recovery.
- If you <b>have not a custom recovery and can't boot into safe mode</b>, you will need to download the lastest [platform-tools](https://developer.android.com/tools/releases/platform-tools) on a PC and enter the command below in CMD (from the extracted <b>"platform-tools"</b> directory) before boot your device, such will disable all the Magisk modules:

> adb wait-for-device shell magisk --remove-modules

# ❗Disclaimer
<b>I am not responsible for anything that happens to your device, make sure you know how to recover it.</b>

# ❤️ Credits
### Special thanks to:

- [Android Open Source Project (AOSP)](https://source.android.com) for Android source code.
- [Substratum](https://github.com/substratum/substratum) for references on building overlays.
- [@DrDisagree](https://github.com/Mahmud0808) for allowing me to implement part of the [Iconify](https://github.com/Mahmud0808/Iconify) code related to overlay management and the installation of the module, essential for the operation of the app.

# ❓ FAQ
<details>
  <summary>Why Camaleon is not in Google Play?</summary>

  - The overlay compilation process runs on external storage, so it requires permission to access all files, which is a sensitive permission according to GP policies. I'm likely to be able to convince Google in the near future that this permission is necessary for Camaleon to work, or find a way to waive it instead. For now, you can get the Camaleon app from [Releases](https://github.com/ArzJo/Camaleon/releases) page.
</details>
<details>
  <summary>How does the Camaleon app work?</summary>

  - The Camaleon app works through the management of RROs, which is based on the Substratum and Iconify theme engines.  
</details>
