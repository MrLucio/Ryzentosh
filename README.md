# Ryzentosh

![Mac OS version](https://img.shields.io/badge/Big%20Sur-11.6.2-informational) \
![Open Core version](https://img.shields.io/badge/Open%20Core-0.7.5-informational) \
![License](https://img.shields.io/github/license/MrLucio/Ryzentosh)

## Disclaimer
Use it at your own risk.

I take no responsibility for how you choose to use the files available in this repository, it comes with no guarantee.

## Screenshots
### Big Sur (11.16.2)
Login screen | System Info screen 
:-------------------------:|:-------------------------:
![](img/Big%20Sur/login.png)  |  ![](img/Big%20Sur/system.png)

## Specifications
| **Component** | **Model** |
| ------------- | --------- |
| CPU | AMD Ryzen 3700x |
| Motherboard | MSI B450 GAMING PRO CARBON MAX WIFI |
| GPU | AMD Radeon R9 380 4GB |
| RAM | 2x 8GB Corsair Vengeance (3200 MHz) |
| Disk | HDD WesternDigital Blue SATA |
| LAN | Intel® I211AT Gigabit LAN controller |
| WiFi / Bluetooth | Intel® Dual Band Wireless-AC 9260 |


## Compatibility
If some of your components are not the same as the ones listed here then be aware that this configuration might not work properly on your hardware.

- Non-Ryzen CPUs won't probably work properly
- All motherboars should work out of the box, but some may not recognize USB devices [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#usb)]
- If you plan to use a NVME storage you should use NVMEFix [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#extras)] [[Download](https://github.com/acidanthera/NVMeFix/releases)]
- Different LAN Chipsets will probably work fine as long as they are Intel's\
Same goes for WiFi / Bluetooth

Remember to add any additional Kext to your config.plist [[Guide](https://dortania.github.io/OpenCore-Install-Guide/config.plist/#adding-your-ssdts-kexts-and-firmware-drivers)]

## Checklist
- [X] Ethernet connection
- [X] WiFi and Bluetooth connection
- [X] iCloud

## ACPI, Drivers and Kexts
### ACPI
- SSDT-EC-USBX-DESKTOP [[Guide](https://dortania.github.io/Getting-Started-With-ACPI/ssdt-platform.html#desktop)] [[Download](https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-EC-USBX-DESKTOP.aml)]
### Drivers
- HfsPlus [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#universal)] [[Download](https://github.com/acidanthera/OcBinaryData/blob/master/Drivers/HfsPlus.efi)]
- OpenCanopy [[Guide](https://dortania.github.io/OpenCore-Post-Install/cosmetic/gui.html)] [[Download](https://github.com/acidanthera/OpenCorePkg/releases)]
- OpenRuntime [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#universal)] [[Download](https://github.com/acidanthera/OpenCorePkg/releases)]
### Kexts
#### Must haves
- VirtualSMC [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#must-haves)] [[Download](https://github.com/acidanthera/VirtualSMC/releases)]
- Lilu [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#must-haves)] [[Download](https://github.com/acidanthera/Lilu/releases)]
#### Graphics
- WhateverGreen [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#graphics)] [[Download](https://github.com/acidanthera/WhateverGreen/releases)]
#### Audio
- AppleALC [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#audio)] [[Download](https://github.com/acidanthera/AppleALC/releases)]
#### Ethernet
- SmallTreeIntel82576 [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#ethernet)] [[Download](https://github.com/khronokernel/SmallTree-I211-AT-patch/releases)]
#### WiFi and Bluetooth
- AirportItlwm [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#wifi-and-bluetooth)] [[Download](https://github.com/OpenIntelWireless/itlwm/releases)]
- IntelBluetoothFirmware (Firmware and Injector included) [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#wifi-and-bluetooth)] [[Download](https://github.com/OpenIntelWireless/IntelBluetoothFirmware/releases)]
#### Extra
- AMDRyzenCPUPowerManagement [[Download](https://github.com/trulyspinach/SMCAMDProcessor/releases)]
- AppleMCEReporterDisabler [[Guide](https://dortania.github.io/OpenCore-Install-Guide/ktext.html#amd-cpu-specific-kexts)] [[Download](https://github.com/acidanthera/bugtracker/files/3703498/AppleMCEReporterDisabler.kext.zip)]
- RestrictEvents [[Download]()]
- SMCAMDProcessor [[Download](https://github.com/trulyspinach/SMCAMDProcessor/releases)]
