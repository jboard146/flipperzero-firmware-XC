<h1 align="center">Flipper Zero Xtreme Clean</h1>

This firmware is a fork of https://github.com/ClaraCrazy/Flipper-Xtreme code wich according to Clara: "complete overhaul of the [Official Firmware](https://github.com/flipperdevices/flipperzero-firmware), it also features some of the badly implemented ideas from RogueMaster, and lots of awesome code-bits from [Unleashed](https://github.com/DarkFlippers/unleashed-firmware)."

-----
<br>
<h2 align="center">This is a "clean" aka SFW Fork</h2>

I'm not a professional coder not do i claim to be, but Clara's work is good, but I love the cute dolphin in the orgional firmware.

The RogueMaster stuff is a mess and then the whole paywall in Pateron....

This is basicaly my own personal use, but if you like have at it.

----
<br>
<h2 align="center">Install:</h2>

**NOTE: If you are coming from a different FW, it is recommended to delete / clear your "apps" folder on the SD card prior to updating. This folder houses all the .fap files, which do not update to the correct API versions by default if old ones are present (Thanks flipper devs). This does `NOT` remove any of your saved files!**
<br><br>

<h3> Web Updater / Mobile App / Automatic qFlipper Update</h3>

- Go to the latest release from [The releases tab](https://github.com/jboard146/flipperzero-firmware-XC/releases/latest)
- Click the "Web Updater" Button

<br>

-----
<br>

<h3> Manual Update (Because qFlipper loves to break every now and then for no reason at all)</h3>

- Download the latest release (.zip) from [The releases tab](https://github.com/jboard146/flipperzero-firmware-XC/releases/latest)
- Extract the archive. This is now your new Firmware folder
- Open [qFlipper](https://flipperzero.one/update), head to `SD/Update` and simply move the firmware folder there
- On the Flipper, hit the `Arrow Down` button, this will get you to the file menu. Hit `Arrow Left` once, and then simply search for your updates folder
- Inside that folder, select the Firmware you just moved onto it, and run the file thats simply called `Update`

- Enjoy!

----
<br>
<h2 align="center">Build it yourself:</h2>

```bash
To download the needed tools:
$ git clone --recursive https://github.com/jboard146/flipperzero-firmware-XC

To flash directly to the Flipper (Needs to be connected via USB, qFlipper closed)
$ ./fbt flash_usb

To just compile firmware
$ ./fbt updater_package

If building FAPS:
$ ./fbt fap_dist

If building image assets:
$ ./fbt resources icons dolphin_ext
