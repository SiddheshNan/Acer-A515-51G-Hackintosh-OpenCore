# Acer-A515-51G-Hackintosh-OpenCore

[![Join the chat at https://gitter.im/Acer-A515-51G-Hackintosh](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/Acer-A515-51G-Hackintosh/community)

For Clover Bootloader with MacOS X Support, Visit this [Repo](https://github.com/SiddheshNan/Acer-A515-51G-Hackintosh).
---

#### Supports MacOS 11.0.x

<p align="center">
  <img src="https://i.imgur.com/q7VSJPa.png" alt="Specs">
</p>


## What's Working...
 - [x] Audio & headphone jack
 - [x] CPU Speedstep
 - [x] iGPU with disabled dGPU
 - [x] Fully Functional QE/CI Enabled Graphics
 - [x] Battery Management
 - [x] ACPI Display brightness with hot keys / slider
 - [x] Ethernet
 - [x] HDMI + Audio
 - [x] Smart Touchpad + Gestures (using Basic Mode)
 - [x] WebCam
 - [x] Usb 3.0 + Type C
 - [x] WiFi (2.4 + 5GHz) by using BCM94352z
 - [x] Native hotkey support with Fn keys


 ### Known Issues
- Bcm94352z Bluetooth (bcm20702a0) not working
- Trackpad in Advance Mode, Only Basic mode works (but with all with gestures)!

### Not Tested
-  Sleep + Wake
 - Internal SD card Reader

### Important
 Please add `SystemSerialNumber`, `SystemUUID` and `MLB`.


## Installation

 ### BIOS Settings
* *Security* → Set supervisor password (to disable secure boot)
* *Security* → Password on boot → **Disable**
* *Boot* → Secure Boot → **Disable**
* *Boot* → Boot Mode → **UEFI**
* *Main* → Touchpad → Set touchpad mode → **Basic** *TODO: Advance Mode*
* *Main* → Lid Open resume → **Enabled**


###  Basic Installation

- Create a Bootable USB for MacOS by using by Dortania's [OpenCore-Install-Guide](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/).
- Install MacOS to SSD / Hard drive. (While installing, connect USB keyboard and mouse).
- Install [Clover Bootloader](https://github.com/CloverHackyColor/CloverBootloader/releases) into SSD / hard drive.
- Copy **ALL** the Contains of this Repo inside the EFI partition of SSD / Hard drive.
- **[IMPORTANT]** Make sure to Generate system definitions of MacBook pro 15.2 in config.plist file using [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) & add `SystemSerialNumber`, `SystemUUID` and `MLB`.

### Post Installation
- If you have Installed MacOS on SSD, Enable TRIM using following command:

```sh

$ sudo trimforce enable

```


<p align="center">
<b>⭐ Please consider starring this repository if it helped you! ⭐</b>
</p>

