# 💻 OpenCore EFI for Infinix XBOOK B15 BL15A5 (AMD Ryzen™ 5 7430U + AMD Radeon™ Graphics)

> EFI for running macOS on the Infinix XBOOK B15 BL15A5 using OpenCore bootloader.

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
| Audio            | Realtek ALC69                    |
| macOS Version    | macOS Sonoma 14.8                |
| OpenCore Version | 1.0.5                            |
| SMBIOS           | MacBookPro16,2                   |

---

## ✅ What's Working

- [X] Boot and Installation
- [X] CPU Power Management
- [X] GPU Acceleration (iGPU)
- [X] Audio (Speakers & Microphone)
- [X] Internal Display (Brightness Control)
- [ ] Wi-Fi
- [ ] Bluetooth
- [X] Battery Status
- [X] Sleep / Wake
- [X] USB Ports
- [X] Touchpad
- [X] Keyboard (Backlight, Fn keys)
- [X] Webcam
- [ ] iServices (iMessage, FaceTime, AirDrop, Handoff)
- [X] Ethernet

---

## ⚠️ Known Issues

- Wi-Fi and Bluetooth
- You tell me

> Wi-Fi is dead, bruh, and this laptop has a soldered PCIe Wi-Fi card.
>
> Alternatively, I use a USB Wi-Fi adapter (TP-Link WL725N), which costs around IDR 90K.
>
> Then, I followed
>
> [this guide](https://github.com/chris1111/Wireless-USB-OC-Big-Sur-Adapterhttps:/).

## 🛠️ Required BIOS Settings

Please update to the latest BIOS and configure the following:

- **Fast Boot**: Disabled
- **Secure Boot**: Disabled
- **IOMMU**: Disabled
- **CSM (Compatibility Support Module)**: Disabled
- **Above 4G Decoding**: Enabled

---

## 🔧 Tools and Kexts Used

- **Bootloader**: OpenCore v1.0.5 release
- **ACPI**:
  - SSDT-AL50
  - SSDT-EC
  - SSDT-PLUG-ALT
  - SSDT-PNLF
  - SSDT-USB-Reset
  - SSDT-USBX
  - SSDT-XOSI
- **Kexts**:
  - Lilu.kext (v1.7.1)
  - VirtualSMC.kext (+ SMCBatteryManager.kext, SMCLightSensor.kext) (v1.3.7)
  - SMCProcessorAMD.kext (v1.0.1)
  - SMCRadeonSensors.kext (v2.3.1)
  - NootedRed.kext (v1.0.0)
  - AppleALC.kext (v1.9.5)
  - RealtekRTL8111.kext (v2.5.0)
  - VoodooPS2.kext (v2.3.7)
  - VoodooI2C.kext (+ VoodooI2CHID.kext) (v2.9.1)
  - VoodooSMBus.kext (v2.2)
  - NVMeFix.kext (v1.1.3)
  - AppleMCEReporterDisabler.kext (v1.0)
  - ForgedInvariant.kext (v1.2.0)
  - RestrictEvents.kext (v1.1.6)
  - ECEnabler.kext (v1.0.6)
  - BrightnessKeys.kext (v1.0.3)

---

## 💼 SMBIOS Info

- **Model**: MacBookPro16,2
- **Serial Number**: Generate your own
- **Board Serial Number**: Generate your own
- **SmUUID**: Generate your own
- **MLB**: Generate your own

❗ *Please generate your own unique SMBIOS using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) before using this EFI.*

---

## 💡 Notes

- This EFI is configured for macOS Sonoma but should work with other macOS versions.
- Always test with a USB before replacing your current EFI.
- This is provided as-is. Make sure to backup your data before using.

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

## 📎 Download

Grab the latest release [here](https://github.com/kodeaqua/opencore-infinix-xbook-b15/releases)

---

## 🍹 Buy me some Cendol~

If you find my work helpful and feel like showing support, you can send me some cendol at [here](https://teer.id/kodeaqua).

---
