# 💻 OpenCore EFI for Infinix XBOOK B15 BL15A5 (AMD Ryzen™ 5 7430U + AMD Radeon™ Graphics)

EFI for running macOS on the Infinix XBOOK B15 BL15A5 using OpenCore bootloader.

---

## ❗ READ THIS
- *Do this at your own risk. I am not responsible if your laptop becomes bricked or if anything bad happens.*
- *I do not recommend installing this as the primary OS on your laptop. There are many issues, so please use Microsoft Windows as your primary OS, as it is more stable.*
- *This is not OpenCore-related, but I strongly advise you not to modify BIOS settings (this laptop has unlocked engineer-level settings). I accidentally misconfigured the BIOS and my laptop became bricked with no recovery options. I had to send it to the official service centre for repairs, which took one week. They said the problem was with the motherboard and replaced it.*

---

## 🖥️ System Information


| Component        | Details                          |
| ------------------ | ---------------------------------- |
| Laptop Model     | Infinix XBOOK B15 BL15A5         |
| CPU              | AMD Ryzen™ 5 7430U              |
| GPU              | Integrated AMD Radeon™ Graphics |
| RAM              | 16GB DDR4 @ 3200MHz              |
| Storage          | 512GB NVMe SSD                   |
| Wi-Fi / BT       | Soldered Realtek RTL8821CE       |
| LAN              | Realtek RTL8111                  |
| Audio            | Realtek ALC269VC                 |
| macOS Version    | macOS Sequoia 14.8                |
| OpenCore Version | 1.0.6                            |
| SMBIOS           | MacBookPro16,2                   |

---

## ✅ What's Working

- [X] Boot and Installation
- [X] CPU Power Management
- [X] GPU Acceleration (iGPU) (see Known Issues)
- [X] Audio (Speakers & Microphone)
- [X] Internal Display (Brightness Control)
- [X] Bluetooth
- [X] Battery Status
- [X] Sleep / Wake
- [X] USB Ports
- [X] Touchpad
- [X] Keyboard (Backlight, Fn keys)
- [X] Webcam
- [X] Ethernet
- [ ] Wi-Fi and Location Service
- [ ] iServices (iMessage, FaceTime, AirDrop, Handoff)

---

## ⚠️ Known Issues

- Wi-Fi
- Location Service
- Rendering
- You tell me

> Wi-Fi is dead, bruh, and this laptop has a soldered PCIe Wi-Fi card. Alternatively, I use a USB Wi-Fi adapter (TP-Link WL725N), which costs around IDR 90K. Then, I followed [this guide](https://github.com/chris1111/Wireless-USB-OC-Big-Sur-Adapter).
> Location Services are not working because they require a macOS-compatible Wi-Fi card.
> Rendering is actually fast and good, but when you run apps or games like Steam or PCSX2, you will see artifacting, and the system may freeze for a few moments. I don’t know why. The same issue also happens in Google Chrome.

## 🛠️ Required BIOS Settings

Please update to the latest BIOS and configure the following:

- **Fast Boot**: Disabled
- **Secure Boot**: Disabled
- **IOMMU**: Disabled
- **CSM (Compatibility Support Module)**: Disabled
- **Above 4G Decoding**: Enabled
- **UMA/GPU VRAM/GPU Memory**: UMA Game Optimized

---

## 💡 Notes

- This EFI is configured for macOS Sonoma but should work with other macOS versions.
- Always test with a USB before replacing your current EFI.
- This is provided as-is. Make sure to backup your data before using.
- Please generate your own unique SMBIOS using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) before using this EFI.

---

## 🧩 Credits

- OpenCore Team
- Dortania Guide: https://dortania.github.io/
- [Acidanthera](https://github.com/acidanthera)
- [CorpNewt](https://github.com/corpnewt)
- [macos86](https://github.com/macos86)
- [CheffKissInc](https://github.com/ChefKissInc)
- [Mieze](https://github.com/Mieze)
- [VoodooSMBus](https://github.com/VoodooSMBus)
- [averycblack](https://github.com/averycblack)
- [AMD-OSX](https://github.com/AMD-OSX/AMD_Vanilla)
- [mikigal](https://github.com/mikigal/ryzen-hackintosh)
- Other contributors, repos, Hackintosh forums

---

## 🍹 Buy me some Cendol~

If you find my work helpful and feel like showing support, you can send me some cendol at [here](https://teer.id/kodeaqua).

---
