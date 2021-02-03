# ASRock Z390M-ITX/ac macOS Big Sur 11.1 OpenCore EFI

**Table of contents**
- [ASRock Z390M-ITX/ac macOS Big Sur 11.1 OpenCore EFI](#asrock-z390m-itxac-macos-big-sur-111-opencore-efi)
  - [Images](#images)
  - [Hardware](#hardware)
  - [Wi-Fi and Bluetooth module](#wi-fi-and-bluetooth-module)
  - [What Works](#what-works)
  - [What I have not tested yet](#what-i-have-not-tested-yet)
  - [SMBIOS](#smbios)

## Images

System

![system information](images_in_readme/system_info.png "System Information")

GPU

![gpu acceleration](images_in_readme/gpu_acceleration.png)

## Hardware

| Item        | Model                                  |
| ----------- | -------------------------------------- |
| CPU         | [Intel Core-5 9600KF](https://ark.intel.com/content/www/us/en/ark/products/190884/intel-core-i5-9600kf-processor-9m-cache-up-to-4-60-ghz.html)                    |
| MotherBoard | [ASRock Z390M-ITX/ac](https://www.asrock.com/mb/Intel/Z390M-ITXac/index.asp)                    |
| Wi-Fi       | BCM94360CS2 + NGFF-convertor           |
| GPU         | [Sapphire RX560XT 4G D5](https://www.anandtech.com/show/14079/amd-launches-china-only-radeon-rx-560xt)                 |
| RAM         | G.SKILL 32GB(16GB x 2) 2400MHz DDR4    |
| SSD1        | WD_BLACK SN750 NVME 500GB for Hackintosh |
| SSD2        | HP S700 500GB (SATA3.0) |
| Power       | FSP MS450                              |
| Cooler      | be Quiet! BK008 Pure Rock Slim         |
| Chassis     | Mechanic master cube C24               |


## Wi-Fi and Bluetooth module

ASRock Z390M-ITX/ac has a Intel Wi-Fi module(M.2 E-key) which can not driven by macOS. I replaced it by a `BCM94360CS2`.

## What Works

- GPU with hardware acceleration
- Audio
- Ethernet
- Wi-Fi(2.4GHz and 5GHz)
- Bluetooth
- USB 2.0, USB 3.0, type-C, front panel USB 3.0
- Airdrop
- CPU boost
- Sleep [Michael-kj](https://github.com/michael-kj) have tested.

## What I have not tested yet

- iMessage

## SMBIOS
I have remove my SMBIOS info from config.plist. You should generate your own SMBIOS info use [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS).
