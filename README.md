# macOS for Lenovo ThinkPad T440p (February 1, 2020)
![T440p](https://www.pc-canada.com/dd2/img/item/A-1500x1500/548012.jpg)

This project is to give the T440p a complete and functional build of macOS Catalina `10.15.3` using the guide from [here](https://github.com/jloisel/t440p) with modified kexts.

## My Specs
**Model:** T440p 20AWS09700

**Bios:** Modded v2.54 (Modified for removal of wifi card whitelist and advanced features)

**CPU:** 2.79GHz Intel i7-4900MQ

**GPU:** Intel HD Graphics 4600 1536MB (0x0412)

**RAM:** 1600MHz Kingston Hyper X Impact 16GB Dual Channel DDR3

**Display:** 14" Innolux N140HCE-EN1 Rev.C2 IPS Anti-Glare FHD, 1920x1080, 60Hz

**Storage:** 
- SATA KingSpec NT-512 SSD 512GB
- SATA Samsung 860 Pro SSD 256GB

**Partition Type:** APFS (TRIM automatically enabled by APFS)

**SD Card Reader:** Realtek SD Card Reader

**Wifi:** Broadcom DW1560 (0x14E4)

**Bluetooth:** Broadcom DW1560 with firmware `v14 c5668`

**Bootloader:** Clover v2.5k_r5103

## Note
Your ThinkPad may or may not have the exact specs as mine. Results may vary. If you need help, please ask.
If you use a USB wifi adapter look for drivers from that model.

## Tested Configurations
- macOS 10.15.3 (19D76)
- BIOS v2.54

# What Works
- Audio
- Headphone Jack
- Keyboard
- Keyboard Brightness
- Battery Manager
- USB A Ports
- Trackpad, with gestures
- Microphone
- Display Brightness
- Wifi
- Bluetooth
- Optical Drive

# What doesn't Work
- Waking from sleep (Unless you unload the AudioHDA.kext before putting it to sleep)
- SD Card Reader

# Bugs
- Booting up macOS, the wifi module takes some time to initiate

# Pre-Installation
1. Replace original wifi chipset with a DW1560 (Recommended) or use a USB wifi adapter (Not recommended)
2. You will have to wipe the entire disk
3. Make sure to have a modded BIOS with wifi whitelist removed
4. Change your BIOS settings:
     - **Startup Tab**
      - `UEFI/Legacy Boot` Both
      - `UEFI/Legacy Priority` UEFI First
      - `CSM Support` Yes

5. For Installation go to the [wiki]().

# Undervolting
- Follow the [guide](https://www.insanelymac.com/forum/topic/331775-guide-how-to-undervolt-your-haswell-and-above-cpu/).

## Credits
- jloisel (https://github.com/jloisel/t440p)
