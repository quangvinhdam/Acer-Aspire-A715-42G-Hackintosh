<h1 align="center"> Hackintosh on Acer Aspire A715-42G</h1>

<p align="center">
  A macOS experiment on an AMD Ryzen laptop powered by OpenCore.
</p>

---

## 🖥️ Specifications

| Component        | Details                                         |
|------------------|--------------------------------------------------|
| **Model**        | Acer Aspire A715-42G                            |
| **CPU**          | AMD Ryzen 5 5500U (6 cores / 12 threads)        |
| **iGPU**         | AMD Radeon Graphics (Lucienne)                 |
| **dGPU**         | NVIDIA GeForce GTX 1650 (disabled in macOS)     |
| **RAM**          | 24 GB DDR4 (16 GB Samsung + 8 GB Hynix) @ 3200MHz |
| **Storage**      | WDC SN530 NVMe 256GB                            |
| **Audio**        | Realtek ALC255                                  |
| **Wi-Fi/BT**     | Broadcom 802.11ac (macOS compatible)            |
| **Ethernet**     | Realtek PCIe GbE Controller                     |
| **Monitor**      | AUO B156HAN02.1 – 15.6" FHD                     |

---

## ✅ What's Working

- AMD Kernel Patches (via OpenCore)
- macOS Boot (Monterey / Ventura with legacy patches)
- Basic GPU Acceleration (experimental with AMDGPU kexts)
- Audio (with layout-id via AppleALC)
- USB 2.0 / 3.0 Ports (with UTBMap.kext & USBToolbox.kext)
- Ethernet (with RealtekRTL8111.kext)
- Brightness & Volume Keys (with custom ACPI patches)
- Touchpad (via VoodooI2C / ELAN support)
- HDMI Output
- SSD NVMe Support

---

## ❌ Not Working / Experimental

- Sleep / Wake
- AirDrop / Continuity (limited due to AMD)
- NVIDIA GTX 1650 (macOS doesn't support recent NVIDIA dGPUs)
- Native Power Management (partial, ACPI tuning needed)
- DRM Video Playback (e.g. Netflix in Safari may not work)

---

## 🛠️ Tools & Configuration

- **Bootloader**: OpenCore 0.9.x  
- **macOS Version**: Monterey / Ventura  
- **Kernel Patches**: AMD Vanilla Patches  
- **Config Source**: Dortania AMD Guide  
- **SSDTs**: Extracted with SSDTime
- **Kexts**:
  - `Lilu.kext`
  - `WhateverGreen.kext`
  - `AppleALC.kext`
  - `VirtualSMC.kext`
  - `VoodooI2C.kext`, `VoodooI2CHID.kext`
  - `UTBMap.kext`
  - `RealtekRTL8111.kext`

---

## 🙏 Credits

- 🍏 **Apple** – for macOS  
- 🛠️ **Acidanthera** – OpenCore, Lilu, and associated kexts  
- 🧠 **Dortania Team** – for AMD Hackintosh documentation  
- 🧰 **Corpnewt** – for USBToolBox & tools  
- 👨‍💻 AMD Hackintosh Community – for ongoing support  

