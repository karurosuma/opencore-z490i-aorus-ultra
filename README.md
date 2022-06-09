# OpenCore Monterey for Z490i Aorus Ultra

## Spec
* Motherboard: Gigabyte Z490i Aorus Ultra
* CPU: Intel Core i7-10700K
* GPU: Sapphire RX6600 Pulse 8GB
* RAM: 64GB
* LAN: Intel i225-V
* WLAN: Intel Wi-Fi 6 AX201
* OpenCore: 0.8.1
* macOS 12.4

# Getting Started
1. Update i225-v firmware to latest version.<br>
   https://www.gigabyte.com/tw/Motherboard/Z490I-AORUS-ULTRA-rev-1x/support#support-dl-driver-lan
2. Create macOS USB installer.<br>
   https://support.apple.com/en-us/HT201372
3. Mount EFI volume and paste `EFI/` folder into `/Volumes/EFI/`.
4. Rename `config.plist_sample` to `config.plist`.
5. Follow below instruction to update the `Platforminfo` section in `config.plist`.<br>
   https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#platforminfo
6. Boot from USB.

# BIOS Settings
* Version: F21a