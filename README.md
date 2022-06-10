# OpenCore Monterey for Z490i Aorus Ultra

# Getting Started
## On Windows
1. Update i225-v firmware to latest version.<br>
   https://www.gigabyte.com/tw/Motherboard/Z490I-AORUS-ULTRA-rev-1x/support#support-dl-driver-lan
2. Create USB Mapping using `USBToolbox`.<br>
   https://github.com/USBToolBox/tool
## On macOS
2. Create macOS USB installer.<br>
   https://support.apple.com/en-us/HT201372
3. Mount EFI volume and paste `EFI/` folder into `/Volumes/EFI/`.
4. Replace your generated `UTBMap.kext` on Windows in `/Volumes/EFI/OC/Kexts/`.
5. Follow below instructions to update the `Platforminfo` section in `config.plist`.<br>
   https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#platforminfo<br>
   https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#using-gensmbios
6. Boot from USB.

# Spec
* Motherboard: Gigabyte Z490i Aorus Ultra
* Motherboard BIOS Version: F21a 
* CPU: Intel Core i7-10700K
* GPU: Sapphire RX6600 Pulse 8GB
* RAM: 64GB
* LAN: Intel i225-V
* WLAN: Intel Wi-Fi 6 AX201
* OpenCore: 0.8.1
* macOS 12.4

# BIOS Settings
| Options | Status |
| --- | --- |
| Above 4G Decoding | Enabled |
| CFG-Lock | Disabled |
| CSM | Disabled |
| EHCI/XHCI Hand-off | Enabled |
| Intel Platform Trust Technology | Enabled |
| Intel SGX | Software Controlled |
| OS Type | Windows 10 |
| Secure Boot | Disabled |
| VT-d | Enabled |

# Preview
![About This Mac](./preview.png)
