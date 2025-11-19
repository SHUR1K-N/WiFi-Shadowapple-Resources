# Wi-Fi Shadowapple Resources
Created this info-dump repo as an extension to my YouTube video about the **Wi-Fi Shadowapple**. Hoping it helps people that have questions about supported chipsets, configurations, errors, etc..

*I'll keep updating this as much as possible. If you run into problems using this project, open up a GitHub Issue on the [main "Wi-Fi Prineapple Clone" project repo by xchwarze](https://github.com/xchwarze/wifi-pineapple-cloner).*

## Table of Contents
- [Guide Videos](https://github.com/SHUR1K-N/wifi-shadowapple-resources#guide-videos)
	- [Hardware & installation (easiest method)](https://github.com/SHUR1K-N/wifi-shadowapple-resources#hardware--installation-easiest-method)
	- [Configuration, tips, chipsets, troubleshooting, and more](https://github.com/SHUR1K-N/wifi-shadowapple-resources#upgrade--configuration-tips-chipsets-troubleshooting-and-more)
- [Parts](https://github.com/SHUR1K-N/wifi-shadowapple-resources#parts)
- [Chipsets](https://github.com/SHUR1K-N/wifi-shadowapple-resources#chipsets)
  - [2.4GHz / dual-band adapter decision](https://github.com/SHUR1K-N/wifi-shadowapple-resources#how-do-i-know-whether-i-should-get-a-24ghz-or-dual-band-adapter)
  - [Supported 2.4GHz chipsets](https://github.com/SHUR1K-N/wifi-shadowapple-resources#supported-24ghz-chipsets)
  - [Supported 2.4GHz + 5GHz (dual-band) chipsets](https://github.com/SHUR1K-N/wifi-shadowapple-resources#supported-24ghz--5ghz-dual-band-chipsets)
  - [Tested & confirmed as NOT supported](https://github.com/SHUR1K-N/wifi-shadowapple-resources#tested--confirmed-as-not-supported)
  - [Personally confirmed & cheapest adapter links](https://github.com/SHUR1K-N/wifi-shadowapple-Resources#personally-ordered--verified-adapter-links-non-affiliate)
- [Troubleshooting](https://github.com/SHUR1K-N/wifi-shadowapple-resources#troubleshooting)
  - ["Status:Monitor interface won't start! Try to run airmon-ng..."](https://github.com/SHUR1K-N/wifi-shadowapple-resources#statusmonitor-interface-wont-start-try-to-run-airmon-ng-error-message)
  - [Can't connect to open AP](https://github.com/SHUR1K-N/wifi-shadowapple-resources#cant-connect-to-open-ap)
  - [Can't format USB flash drive / USB flash drive unrecognized](https://github.com/SHUR1K-N/wifi-shadowapple-Resources#cant-format-usb-flash-drive-or-usb-flash-drive-not-recognized)
  - [Going back to stock firmware](https://github.com/SHUR1K-N/wifi-shadowapple-Resources#going-back-to-the-shadows-stock-firmware)

## Guide Videos
### Hardware & installation — easiest method
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/67sGUzKJ8IU/maxresdefault.jpg)](https://youtu.be/67sGUzKJ8IU)

### Upgrading the Shadowapple for MAX hackability
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/pHtpso21P0o/maxresdefault.jpg)](https://www.youtube.com/watch?v=pHtpso21P0o&t=307s)

---
---
# Parts
* GL.iNet Shadow (AR300M16-Ext) router ([Amazon](https://amzn.to/3Idqc9g))
* 2× Wi-Fi adapters with [supported chipsets](https://github.com/SHUR1K-N/wifi-shadowapple-resources#chipsets)
* USB flash drive
* USB hub with a minimum of 3 ports [Amazon](https://amzn.to/4oZd2MX)

---
---
# Chipsets
The Wi-Fi Shadowapple is capable of 5GHz sniffs & attacks as well if a 5GHz adapter with a _supported_ chipset is used.

## How do I know whether I should get a 2.4GHz, or dual-band adapter?

Your selection of bands (2.4GHz or dual-band) would depend on the wireless awareness in your region/hood (in terms of security, adaptation to new technology, etc.).

Most *traditional* APs operate only on 2.4GHz.

Most *modern* APs are ″dual-band″ ― they operate on both 2.4GHz (for long range + smart home devices) and 5GHz (for higher speeds at short ranges).

The *latest* APs even go 6GHz (even higher speeds).

A good starting point to learning about wireless security―at least personally―would be 2.4GHz. But, of course, it would be best if you also tap into 5GHz since that has now become the new norm.

## Supported 2.4GHz chipsets
As per documentation, some research, and comments on my videos:

* MT7603E/EN
* MT7620A/N
* MT7621
* MT7622
* MT7628
* RT2070 ― _not part of my research; mentioned by someone in the video comments_
* RT2400
* RT2500
* RT2570
* RT2671
* RT2770
* RT2870
* RT3070 ― _confirmed by someone in the video comments_
* RT3071
* RT3072
* RT3370
* RTL8187L/B
* RT5370 ― _personally confirmed + used in my Shadowapple & Mangoapple videos_

## Supported 2.4GHz + 5GHz (dual-band) chipsets
As per documentation, some research, and comments on my videos:

* MT7632U
* MT7613
* MT7610U
* MT7662U/E
* MT7915
* RT3572 ― _confirmed by someone in my Mangoapple repo's Issues_
* RT5572 ― _personally confirmed + confirmed by someone in the video comments, Instagram, and Reddit_
* MT7612U ― _most problematic chipset. Try to stay away from it. In several adapters with this chipset, the adapter's **internal emulated storage** is recognized instead of the **Wi-Fi adapter** itself. If running "lsusb" shows the device ID as "0e8d:2870", then you're in that same boat (the "toast" boat). You should either look into another chipset, or get another adapter with the same chipset and try again, or there are multiple commands & configurations you could try to ″switch″ the adapter's mode from storage to Wi-Fi (but it may get tricky and is not worth it)_

	UPDATE: You can [follow this guide](https://github.com/SHUR1K-N/WiFi-Shadowapple-Resources/issues/4#issue-3398474745) to get your MT7612U out of its storage mode and use it as normal

## Tested & confirmed as NOT supported
As per documentation, some research, and comments on my videos:

* MT7610
* MT7601U
* AR9271
* RTL8811AU/CU
* MT7921AUN

## Personally ordered & verified adapter links (non-affiliate)
### RT5370 (2.4GHz)
* https://www.aliexpress.com/item/2255799898010658.html (1 quantity order limit)
* https://www.aliexpress.com/item/2255799900873717.html
* https://www.aliexpress.com/item/1005008142040949.html ― _confirmed by someone on Patreon_

### RT5572 (dual-band)
* https://www.aliexpress.com/item/3256806000755742.html
* https://www.aliexpress.com/item/1005008392078147.html ― _confirmed by someone on Instagram_
* https://www.aliexpress.com/item/1005009223339345.html ― _confirmed by someone on Patreon_

_If you find any more supported (or unsupported) chipsets during your testing, let me know in the Issues / Discussions / YouTube video comments. Many of us would benefit from your intel and appreciate it!_

---
---

# Troubleshooting
## "Status:Monitor interface won't start! Try to run airmon-ng..." error message
You're most likely using a Wi-Fi adapter with an _unsupported_ chipset. It's just a catch-all error message. Playing around with airmon-ng will not fix this. You'll need an adapter with a [supported chipset](https://github.com/SHUR1K-N/wifi-shadowapple-resources#chipsets).

## Can't connect to open AP
1. ″Filters″ page in the web UI
2. Switch both client and SSID filtering to ″Deny List″
3. "Networking" page, go to the "Config" tab
4. Ensure "Hide Open SSID" is _unchecked_
   > NOTE: the SSID _will_ be broadcasted sometimes even when set to hidden, so uncheck it regardless
6. "Update Access Point" button, regardless of the above setting

## Can't format USB flash drive OR USB flash drive not recognized
1. Verify the USB flash drive is OK by checking it out on your Windows machine first
2. Try manually formatting the USB flash drive (Windows defaults are OK)
3. Re-attach it and see if it gets picked up correctly (″USB & Storage″ section on the ″Advanced″ page of the web UI should show you the model), or you could run ″lsusb″ / ″lsblk″ manually via SSH
4. If it's picked up, try running `wpc-tools format_sd` again (from *outside* the /sd/ directory)
5. If none of the above works, run the following commands:
   
   `opkg update`
   
   `opkg install kmod-usb-storage-uas`
7. Try running `wpc-tools format_sd` again (from *outside* the /sd/ directory)
8. If none of this works, try another USB flash drive altogether (multiple people have reported this fixed it)

## Going back to the Shadow's stock firmware
1. Get to the recovery mode again (as shown in the video)
2. Flash the [original router firmware](https://dl.gl-inet.com/router/ar300m16/stable)
