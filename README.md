# 🍏 Hackintosh EFI – Lenovo IdeaPad Gaming 3 15ARH05 (Ryzen)

This repo contains a fully working EFI setup for macOS **Sequoia** (also compatible with Ventura and Sonoma) on the **Lenovo IdeaPad Gaming 3 15ARH05** with AMD Ryzen 5 4600H and Radeon Vega 6 iGPU.

---

## 💻 Laptop Specifications

| Component            | Details |
|---------------------|---------|
| **Model**            | Lenovo IdeaPad Gaming 3 15ARH05 |
| **CPU**              | AMD Ryzen 5 4600H (Zen 2, 6 cores / 12 threads) |
| **iGPU**             | AMD Radeon RX Vega 6 – ✅ Fully Working |
| **dGPU**             | NVIDIA GTX 1650 – ❌ Disabled (Unsupported) |
| **RAM**              | 16GB DDR4 3200MHz |
| **Storage**          | 512GB NVMe SSD |
| **Display**          | 15.6" FHD 1920×1080 @ 120Hz |
| **Audio**            | Realtek ALC257 – ✅ via AppleALC |
| **WiFi & Bluetooth** | Realtek – ❌ Not Working |
| **Trackpad**         | ✅ Working via VoodooI2C |
| **Battery**          | ✅ Working via SMCBatteryManager |

---

## ✅ What Works

- AMD Ryzen support (with OpenCore kernel patches)
- Radeon Vega 6 iGPU with full hardware acceleration (Metal)
- Internal display (120Hz panel, but limited to 60Hz in macOS)
- Audio via `AppleALC`
- Trackpad via `VoodooI2C`
- Battery stats via `SMCBatteryManager`
- USB ports
- Sleep, shutdown, reboot

## ❌ What Doesn’t Work

- ❌ **NVIDIA GTX 1650**: Not supported in macOS, must remain disabled
- ❌ **WiFi & Bluetooth**: Realtek chip is unsupported in macOS
  - ➤ Recommend replacing with **Broadcom** or **Intel** card (e.g. DW1820A or Fenvi)
  - OR use a **USB WiFi dongle**

---

## 🔧 EFI Files

There are **two EFI folders** provided:

### 🟠 First Boot EFI (Install-Only)

Use this EFI **only for initial macOS installation**. It provides a clean and minimal config to avoid kernel panics or boot hangs. Some features (like audio, gestures, battery) might not work here.

🔗 [Download FIRST_BOOT_EFI](https://github.com/aman71711/Lenovo-IdeaPad-Gaming-3-15ARH05-Hackintosh-EFI-/releases/download/FIRST_BOOT_EFI/FIRST_EFI.zip)

---

### 🟢 After Installation EFI (Full Feature)

Once macOS is installed and you're able to boot to the desktop, **replace the EFI** with this one. It includes:

- Proper device properties
- Fully working audio, battery, and trackpad
- USB map
- Disabled dGPU
- All necessary Ryzen patches

🔗 [Download AFTER_INSTALLATION_EFI](https://github.com/aman71711/Lenovo-IdeaPad-Gaming-3-15ARH05-Hackintosh-EFI-/releases/download/EFI_AFTER_INSTALLATION/AFTER_INSTALLATION_EFI.zip)

---

## 🔌 BIOS Settings (Important)

Ensure your BIOS is configured properly:

- ✅ **Secure Boot** → Disabled  
- ✅ **Fast Boot** → Disabled   
- ✅ **USB Legacy Support** → Enabled  
- ✅ **UEFI Boot Mode** → Enabled

---

## 📚 Guides to Follow

- 💻 **ChefKiss Hackintosh Guide** (for AMD Ryzen):  
  https://github.com/chefkissmac/Ryzen-Hackintosh

- 🧠 **Dortania OpenCore Install Guide**:  
  https://dortania.github.io/OpenCore-Install-Guide/

---

## 📌 Notes & Tips

- During your **first install**, use the `FIRST_BOOT_EFI` to avoid issues.
- Once booted into the macOS desktop, replace it with the `AFTER_INSTALLATION_EFI` for full hardware support.
- Use **ProperTree** to make any plist edits.
- I’ve tested this setup on macOS **Sequoia**, but it should work fine with **Ventura** and **Sonoma** too.
- Remember, NVIDIA dGPU and Realtek WiFi will **not** work.

---

## 🧑‍💻 Credits

- OpenCore Team  
- Dortania for their amazing documentation  
- AMD-OSX Community  
- ChefKiss for the Ryzen Hackintosh base  
- @aman71711 (me) – for testing and EFI build for this specific model

---

Feel free to open an issue or discussion if you need help. I’m happy to assist anyone trying Hackintosh on the same laptop!
