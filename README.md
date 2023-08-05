# OpenCore for Z490i Aorus Ultra
![About This Mac](./preview.png)
## Getting Started
#### On Windows
1. Update i225-v firmware to latest version.
   <br>https://www.gigabyte.com/tw/Motherboard/Z490I-AORUS-ULTRA-rev-1x/support#support-dl-driver-lan
2. Create USB Mapping using `USBToolbox`.<br>
   https://github.com/USBToolBox/tool
#### On macOS
1. Create macOS USB installer.
   <br>https://support.apple.com/en-us/HT201372
2. Mount EFI volume and paste `EFI/` folder into `/Volumes/EFI/`.
3. Replace your generated `UTBMap.kext` on Windows in `/Volumes/EFI/OC/Kexts/`.
4. Rename `config.plist.sample` to `config.plist`.
4. Follow below instructions to update the `Platforminfo` section in `config.plist`.
   <br>https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#platforminfo
   <br>https://dortania.github.io/OpenCore-Post-Install/universal/iservices.html#using-gensmbios
5. Boot from USB.

## Spec
* Motherboard: Gigabyte Z490i Aorus Ultra
* Motherboard BIOS Version: F21a 
* CPU: Intel Core i7-10700K
* GPU: Sapphire RX6600 Pulse 8GB
* RAM: 64GB
* LAN: Intel i225-V
* WLAN: Intel Wi-Fi 6 AX201
* OpenCore: 0.9.3
* macOS 13.0-13.5

## BIOS Settings
| Options | Status |
| --- | --- |
| Above 4G Decoding | Enabled |
| Resizable BAR Support | Auto |
| CFG-Lock | Disabled |
| CSM | Disabled |
| EHCI/XHCI Hand-off | Enabled |
| Intel Platform Trust Technology | Enabled |
| Intel SGX | Software Controlled |
| OS Type | Windows 10 |
| Secure Boot | Disabled |
| VT-d | Enabled |

## Other
### Intel Wi-Fi is not working
Please wait for the update of [Airportitlwm](https://github.com/OpenIntelWireless/itlwm/releases) that support macOS 13.0.

### macOS Monterey support
Please switch to branch [0.8.1](https://github.com/karurosuma/opencore-z490i-aorus-ultra/tree/0.8.1).
