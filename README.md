Resources for HP Probook 430 G3 to run macOS
============================================

- Bootloader version: Opencore 0.7.2
- macOS version: macOS Big Sur 11.5.1 (20G80)
- Windows version: Windows 11 Insider Preview Build 22000.120 for the Beta Channel
![Oops!There was supposed to be an image here](https://user-images.githubusercontent.com/84245065/127441253-b56c7695-999c-433b-a5e7-f42718660080.png)
![Oops!There was supposed to be an image here](https://user-images.githubusercontent.com/84245065/127442252-f3d46091-7b33-4e3c-ae9f-99cd9d630a12.png)
![Oops!There was supposed to be an image here](https://i.imgur.com/EAKVfPD.png)

#### What works
- iGPU acceleration (Intel HD 520)
- Sleep
- Battery Percentage
- Display Brightness
- USB ports
- Internal Camera
- Audio with mute button (Both internal speakers and Microphone) (cx20724)
- Native Power Management/(Also with cpufriend)
- SMBus Controller
- CPU Temperature Monitoring
- VGA (*suprisingly*)
- Dualbooting with Windows 11 Insider Preview Build 22000.120 for the Beta Channel
- iMessage
- Facetime

#### What doesn't work
- Built-In Wifi+Bluetooth (*unsupported*)

#### Specs

| Component      | Brand                                                            |
|----------------|------------------------------------------------------------------|
| **CPU**        | `Intel Core i5-6200U ` |   
| **iGPU**       | `Intel HD Graphics 520 `                                         |
| **Audio**      | `Conexant 20724 - layout 3`                                      |
| **Ethernet**   | `Realtek RTL8111/8168`                                           |
| **OS**         | `macOS Big Sur 11.5.1 (20G80)` and `Windows 11 Insider Preview Build 22000.120 for the Beta Channel`|

#### Not tested
- HDMI output (both audio and video)
- RTS522A PCI Express Card Reader
- (*Ideally both should work, If some is willing to test, create an issue*)

#### To Do
- ~~Add pci devices in system information~~  *done*
- macOS Powerchime (*I don't know what I will do, if you have any suggestions,create an issue*)
- ~~Real Time Clock Loss (RTC)~~ *done*
- Battery Cycle count
- Let me know more

#### Benchmarks
- Geekbench 5 [Multi-core and Single core](https://browser.geekbench.com/v5/cpu/8013906)

#### Important
- In the config.plist, section `PlatformInfo > Generic`, the following fields are currently edited with CHANGEME. Please generate your own serial. 

- This repo can be helpful for other HP Probook/Elitebook series notebooks
 
### Bios Configuration


#### Enable

- Fast Boot
- Runtime Power Management
- Extended Idle Power States
- Deep Sleep
- Power Control
- Turbo Boost
- Virtualization Technology (VTx)
- Hyperthreading
- Multi Processor

 #### Disable
 
- Legacy boot
- Wake when lid is opened
- Wake on USB

#### Having some problem
Create an issue and I'll try to help as many as I can

#### Credits
- [Apple](https://apple.com) for [macOS](https://www.apple.com/macos/big-sur/)
- [Acidanthera](https://github.com/Acidanthera) for [OpenCorepkg](https://github.com/acidanthera/OpenCorePkg) and necessary kexts
- [dortania](https://github.com/dortania) for its detailed guides
- [Corpnewt](https://github.com/CorpNewt) for [USBMap](https://github.com/corpnewt/USBMap)
