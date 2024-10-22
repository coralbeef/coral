# Gigabyte C246M WU4 Hackintosh on OpenCore

## macOS Versions
#### macOS Catalina 10.15.5

## SMBIOS
#### iMac19,1

### What works
- **dGPU** Hardware Accelaration (Final Cut Pro X, VideoProc, Compressor), DRM Content (Apple TV+/Safari Netflix/Amazon Prime)
- **iGPU** Hardware Accelaration (Final Cut Pro X), Apple Sidecar
- **WIFI,Bluetooth** BCM94360CD Required
- **AirDrop, Handoff** BCM94360CD Required
- **USB** All USB3.1/USB2.0 Port
- **Audio** Realtek ALC1220-VB, (layout id: 1)
- **iMessage,FaceTime,Siri** All work fine

### Not works
- Not

### Device Lists
| Device | Model |
|----|----|
| MotherBoard | Gigabyte C246M WU4 |
| CPU | Intel i5 9500 |
| RAM | USCORSAIR 3200 8GB * 2 |
| Video Card | Sapphire RX-590 8GB |
| Sound Card | Realtek ALC894 （MotherBoard）|
| Network Interface Card | PCI-E BCM943602CD (WI-FI + Bluetooth) |
| Hard Disk | Toshiba XG6 256G NVMe SSD |
| Case | Antec P101 Silent Edition |

### Software Version
#### Boot firmware
| Boot  | Versions |
|----|----|
| OpenCore | [Latest release(0.5.9)](https://github.com/acidanthera/OpenCorePkg) |

#### Kext
| Kext | Downloads |
|----|----|
| Lilu | [Latest release(1.4.5)](https://github.com/acidanthera/Lilu) |
| VirtualSMC,SMCProcessor,SMCSuperIO| [Latest release(1.1.4)](https://github.com/acidanthera/VirtualSMC) |
| WhateverGreen | [Latest release(1.4.0)](https://github.com/bugprogrammer/WhateverGreen) Revision |
| AppleALC | [Latest release(1.5.0)](https://github.com/acidanthera/AppleALC) |
| IntelMausi | [Latest release(1.0.3)](https://github.com/acidanthera/IntelMausi) |
| USBInjectAll | [Version: 2018-1108](https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads/?tab=downloads) |
| USBPower | |
| CPUFriend | [Latest release(1.2.0)](https://github.com/acidanthera/CPUFriend) |

#### EFI
| EFI | Downloads |
|----|----|
| HfsPlus | Latest release |https://github.com/acidanthera/OcBinaryData/blob/master/Drivers/HfsPlus.efi
| 

### Where you need to modify

- **Use Tools:** Macserial/GenSMBIOS

![Where you need to modify](https://github.com/SeonMe/ASRock-Hackintosh-OC/raw/master/Images/config_edit.png)
                            https://github.com/corpnewt/GenSMBIOS

- **Use tools:** Hackintool > PCI

![DeviceProperties_Edit](https://github.com/SeonMe/ASRock-Hackintosh-OC/raw/master/Images/DeviceProperties_Edit.png)

### BIOS Settings
- **BIOS Version** F3

| Disabled | Enabled |
|----|----|
| Fast Boot | Above 4G |
| VT-d | EHCI/XHCI Hand-off |
| CSM | OS type: other types |
### Changelog

#### 11/6 2020
* Initial release
