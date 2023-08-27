## Special Note: this repository is not fully finished. But the EFI folder remains usable.

# DELL Latitude E7470 OpenCore & Ventura

<img align="right" src="https://imgur.com/25u1lIk.jpg" width="300">

<a ref="https://github.com/acidanthera/OpenCorePkg"><img src="https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Logos/OpenCore_with_text_Small.png" width="200" height="48"><a/>

## Introduction

<details>
<summary><strong>Getting started</strong></summary>
</br>

**Meet the bootloader:**

- [Why OpenCore?](https://dortania.github.io/OpenCore-Install-Guide/why-oc.html)
- [Dortania's website](https://dortania.github.io)

**Recommended tools:**

- Plist editor: [ProperTree](https://github.com/corpnewt/ProperTree)
- EFI Partition Mounting Script: [MountEFI](https://github.com/corpnewt/MountEFI)

</details>

<details>
<summary><strong>My Hardware</strong></summary>
<br>

| Model              | Dell Latitude E7470                        |
|:-------------------|:-------------------------------------------|
| Processor          | Intel Core i5-6300U @ 2.40GHz 3MB L3 cache |
| Graphics           | Integrated Intel HD Graphics 5500 64 MB    |
| Memory             | 16GB 2133MHz DDR4 SDRAM (Dual channel)     |
| Display            | 14" FHD (1920x1000) - Non-Touch LCD        |
| Storage            | 512GB M.2 SATA SSD                         |
| Audio              | RealTek ALC3235 24-bits                    |
| WLAN + Bluetooth   | Intel® Tri-Band Wireless-AC 18260 867 Mbps |
| LAN                | Ethernet 10/100/1000 Mb/s (RJ-45)          |
| Camera             | 1280x720 FHD Webcam                        |
| Fingerprint Reader | Yes                                        |
| USB 3.0            | USB 3.0 x 2 ports, 1 PowerShare port       |
| SD Card            | SD 4.0                                     |
| Smart Card         | Yes                                        |
| Keyboard           | Backlit Keyboard                           |
| Trackpad           | ALPS Touchpad                              |

</details>

## Status

<details>
<summary><strong>What's working</strong></summary>
</br>

- [x] Intel HD 520 Graphics `incuding graphics acceleration`
- [x] All USB ports
- [x] Internal camera
- [x] WiFi using [AirportItlwm](https://github.com/OpenIntelWireless/itlwm)
- [x] Bluetooth using [IntelBluetoothFirmware and IntelBluetoothInjector](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)
- [x] Shutdown/ Reboot/ Sleep/ Wake
- [x] Speakers and headphones jack
- [x] Intel Gigabit Ethernet
- [x] iMessage, FaceTime, App Store
- [x] miniDP and HDMI with digital audio passthrough (if you experience cursor lags, try turning on and off one of the displays).
- [x] Keyboard and Trackpad(two finger vertical swipes)
- [x] DRM (Works with Google Chrome. Tested with Prime Video and Netflix.)
- [x] SD Card Reader using [Sinetek-rtsx](https://github.com/cholonam/Sinetek-rtsx)

<hr>

- [x] Intel HD 520 Graphics `incuding graphics acceleration`
- [x] All USB ports
- [x] Internal camera
- [x] AirDrop* using [NGFF(M.2) Model BCM94360NG Hackintosh Card](https://www.amazon.com/Hackintosh-M-2-NGFF-BCM94360NG-Continuity/dp/B083YXS7VF)
- [x] WiFi using [NGFF(M.2) Model BCM94360NG Hackintosh Card](https://www.amazon.com/Hackintosh-M-2-NGFF-BCM94360NG-Continuity/dp/B083YXS7VF)
- [x] Bluetooth using [NGFF(M.2) Model BCM94360NG Hackintosh Card](https://www.amazon.com/Hackintosh-M-2-NGFF-BCM94360NG-Continuity/dp/B083YXS7VF)
- [x] Shutdown/ Reboot/ Sleep/ Wake
- [x] Speakers and headphones jack
- [x] Intel Gigabit Ethernet
- [x] iMessage, FaceTime, App Store
- [x] miniDP and HDMI with digital audio passthrough(If you experience cursor lags, try turning on and off one of the displays.)
- [x] Keyboard and Trackpad(two finger vertical swipes)
- [x] DRM(Works with Google Chrome. Tested with Prime Video and Netflix.)
- [x] SD Card Reader using [Sinetek-rtsx](https://github.com/cholonam/Sinetek-rtsx)

<hr>

- [x] Bluetooth using [IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware) (without IntelBluetoothInjector.kext) and BlueToolFixup.kext from: [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)

</details>

<details>
<summary><strong>What's not working</strong></summary>
</br>

- [ ] [Multitouch gestures for ALPS touchpad.](https://github.com/adityabakare/macOS-Dell-Latitude-E7470/issues/1)
- [ ]  Smart Card reader

</details>

<details>
<summary><strong>Make Bluetooth + Wi-Fi work while you're using original Hardware</strong></summary>
</br>

* WiFi using [AirportItlwm](https://github.com/OpenIntelWireless/itlwm)
* Bluetooth using [IntelBluetoothFirmware and IntelBluetoothInjector](https://github.com/OpenIntelWireless/IntelBluetoothFirmware)

</details>

## Current configuration

Up to date on August 20, 2023.
- macOS: Ventura 13.5
- OpenCore: 0.9.3

## Installation

<details>
<summary><strong>Create the USB</strong></summary>
</br>

Follow the [guide on the OpenCore documentation](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/) to create a USB for installation. Choose the operating system you use to create the USB and proceed with the guide. At the end of the Create USB section, OpenCore will ask us to do additional configurations. We don't need to do any of that because the `EFI` folder in this repository provides all necessary configurations we need for installation on Dell Latitude E7470.
</details>

<details>
<summary><strong>Boot and Install macOS</strong></summary>
</br>

- Plug in the USB we created to your Dell computer
- Press the Power button to turn on our computer (if you used the Dell to create the USB, shutdown the computer first)
- Wait and we will see the Apple icon on a black screen with a progress bar at the bottom
- Then, we will see a menu with four options. Make sure select `Disk Utility` to partition your disk appropriately and format the partition for installing macOS into `APFS`. If you are dual booting with other operating systems, an easier way would be to partition the drive beforehand as some formats like NTFS are readonly on macOS.
- Follow the installation steps and configure the preferences to your liking
- Log in to macOS and enjoy

</details>

## Post Installation

<details>
<summary><strong>Booting without USB</strong></summary>
</br>

You need to plug in the installation USB created previously everytime you start macOS after shutdown. If you want to boot without the USB, follow [this guide by OpenCore](https://dortania.github.io/OpenCore-Post-Install/universal/oc2hdd.html#grabbing-opencore-off-the-usb).

</details>

<details>
<summary><strong>Update Instructions</strong></summary>
</br>

- To update from an older version of EFI to the current one, download this repository and replace your EFI folder with this one. Make sure you use your own SMBIOS, the included one is only for reference.

- After update, you can check your current OpenCore version by typing the following line in the Terminal:
```
nvram 4D1FDA02-38C7-4A6A-9CC6-4BCCA8B30102:opencore-version
```
You may see a line printed as follows:
```
4D1FDA02-38C7-4A6A-9CC6-4BCCA8B30102:opencore-version   REL-093-2023-06-12
```
where `REL` means a RELEASE version of OC, `093` means version 0.7.4, and `2023-06-12` is the date of the release.

</details>

<details>
<summary><strong>Fixing iServices</strong></summary>
</br>

- In order to get Apple Services like App Store working, you need to generate your own SMBIOS(The included one is only for reference).

- For more information on how to do that, visit the [Dortania Guide](https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#generate-a-new-serial).

</details>

## Credits

- [Acidanthera](https://github.com/acidanthera) for OpenCore, Lilu and related kexts.
- [OpenIntelWireless](https://github.com/OpenIntelWireless) and others whose kexts I've used.
- [Dortania](https://dortania.github.io) for installation and other guides.
- [Aditya Bakare](https://github.com/adityabakare) - [Big Sur](https://github.com/adityabakare/macOS-Dell-Latitude-E7470)
- [Yosef-y053f01](https://github.com/y053f01) - [Monterey](https://github.com/y053f01/macOS-Monterey-Dell-Latitude-E7470)
- [Smuger12](https://github.com/Smuger12) - [Monterey](https://github.com/Smuger12/Hackintosh_Dell_Latitude_E7470)
- Everyone else who contributed to this repository directly/indirectly.
