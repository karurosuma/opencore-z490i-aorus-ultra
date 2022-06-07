# OpenCore for Z490i Aorus Ultra (Monterey)

## Spec
* Motherboard: Gigabyte Z490i Aorus Ultra 
* GPU: Sapphire RX6600 Pulse 8GB
* OpenCore: 0.8.1

# Getting Started
1. Create macOS USB installer. <br>
   https://support.apple.com/en-us/HT201372
2. Mount EFI volume and paste `EFI/` folder into `/Volumes/EFI/`.
3. Rename `config.plist_sample` to `config.plist`.
4. Follow below instruction to update the `Platforminfo` section in `config.plist`. <br>
   https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#platforminfo
5. Boot from USB.

# BIOS Settings
* Version: F21a