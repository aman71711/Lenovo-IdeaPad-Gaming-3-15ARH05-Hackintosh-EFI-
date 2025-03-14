# EFI for Lenovo IdeaPad Gaming 3 15ARH05

## 💻 Laptop Specifications

| Component           | Specification |
|--------------------|--------------|
| **Model**         | Lenovo IdeaPad Gaming 3 15ARH05 |
| **CPU**           | AMD Ryzen 5 4600H (Zen 2, 6C/12T) |
| **iGPU**          | AMD Radeon RX Vega 6 (Fully Working) |
| **dGPU**          | NVIDIA GTX 1650 (Disabled, unsupported) |
| **RAM**           | 16GB DDR4 3200MHz |
| **Storage**       | 512GB NVMe SSD |
| **Display**       | 15.6" 1080p 120Hz |
| **Audio**         | Realtek ALC257 (AppleALC) |
| **WiFi & Bluetooth** | Realtek (Not working, unsupported) |
| **Trackpad**      | Working (VoodooI2C) |
| **Battery & Power Management** | Working (SMCBatteryManager) |

🔧 What Works & What Doesn't
✅ Everything except WiFi & Bluetooth (because Realtek chips aren’t supported)
❌ No NVIDIA GPU acceleration (as expected)

For WiFi and Bluetooth, I’m considering getting a USB adapter or replacing the internal card with a Broadcom or Intel one.

Overall, macOS sequoia runs smoothly, and I’m happy with the performance! 🚀 If anyone else is attempting this on the same laptop, feel free to ask for help.

Follow ChefKiss’s guide: ChefKiss Hackintosh Guide
Follow Dortania’s OpenCore guide: Dortania Guide
Use my EFI folder 

