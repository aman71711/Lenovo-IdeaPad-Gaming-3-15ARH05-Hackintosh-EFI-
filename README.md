# Lenovo-IdeaPad-Gaming-3-15ARH05-Hackintosh-EFI-
EFI for running macOS Sequoia on Lenovo IdeaPad Gaming 3 15ARH05 (Ryzen 5 4600H, Vega 6 iGPU) using OpenCore. Fully working except for WiFi &amp; Bluetooth (Realtek unsupported).


💻 Laptop Specifications
Component	Specification
Model	Lenovo IdeaPad Gaming 3 15ARH05
CPU	AMD Ryzen 5 4600H (Zen 2, 6C/12T)
iGPU	AMD Radeon RX Vega 6 (Fully Working)
dGPU	NVIDIA GTX 1650 (Disabled, unsupported)
RAM	16GB DDR4 3200MHz
Storage	512GB NVMe SSD
Display	15.6" 1080p 120Hz
Audio	Realtek ALC257 (AppleALC)
WiFi & Bluetooth	Realtek (Not working, unsupported)
Trackpad	Working (VoodooI2C)
Battery & Power Management	Working (SMCBatteryManager)
✅ What Works
macOS boots and runs smoothly
AMD Radeon Vega 6 graphics acceleration
Audio (ALC257) via AppleALC
Trackpad gestures & keyboard
Battery management & sleep/wake
USB ports (patched with USBMap)
Ethernet (RTL8111)
❌ What Doesn't Work
WiFi & Bluetooth (Realtek is not supported)
NVIDIA GTX 1650 (Disabled, macOS does not support NVIDIA on modern macOS versions)
