# DELL Latitude E7470 OpenCore & Ventura

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
| Processor          | Intel Core i5-6300U                        |
| Graphics           | Integrated Intel HD Graphics 520           |
| Memory             | 16GB 2133MHz DDR4 SODIMM (Dual channel)    |
| Display            | 14" WQHD (2560x1440) with ELAN Touchscreen |
| Storage            | Sandisk 512GB M.2 SATA SSD                 |
| WLAN + Bluetooth   | Intel Dual Band Wireless-AC 8260           |
| Camera             | 1920x1080 FHD Webcam                       |
| Fingerprint Reader | No                                         |
| Soundcard          | Realtek ALC293                             |
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
- [x] miniDP and HDMI with digital audio passthrough(If you experience cursor lags, try turning on and off one of the displays.)
- [x] Keyboard and Trackpad(two finger vertical swipes)
- [x] DRM(Works with Google Chrome. Tested with Prime Video and Netflix.)
- [x] SD Card Reader using [Sinetek-rtsx](https://github.com/cholonam/Sinetek-rtsx)

<hr>

- [x] Intel HD 520 Graphics **`including graphics acceleration`**
- [x] All USB ports
- [x] Internal camera
- [x] WiFi using [AirportItlwm](https://github.com/OpenIntelWireless/itlwm)
- [x] Bluetooth using [IntelBluetoothFirmware](https://github.com/OpenIntelWireless/IntelBluetoothFirmware) (without IntelBluetoothInjector.kext) and BlueToolFixup.kext from: [BrcmPatchRAM](https://github.com/acidanthera/BrcmPatchRAM)
- [x] Shutdown/Reboot/Sleep/Wake
- [x] Speakers and headphones jack
- [x] Intel Gigabit Ethernet
- [x] iMessage, FaceTime, App Store
- [x] miniDP and HDMI with digital audio passthrough (If you experience cursor lags, try turning on and off one of the displays.)
- [x] Keyboard and Trackpad (two finger vertical swipes)
- [x] DRM (Works with Google Chrome. Tested with Netflix.)
- [x] SD Card Reader using [Sinetek-rtsx](https://github.com/cholonam/Sinetek-rtsx)

</details>

<details>
<summary><strong>What's not working</strong></summary>
</br>

- [ ] Multitouch gestures for ALPS touchpad.([#1](https://github.com/adityabakare/macOS-Dell-Latitude-E7470/issues/1))

<hr>

- [ ] [Multitouch gestures for ALPS touchpad.](https://github.com/adityabakare/macOS-Dell-Latitude-E7470/issues/1)

</details>
