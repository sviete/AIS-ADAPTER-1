# AIS-ADAPTER-1 Ethernet Zigbee Adapter's FIRMWARE

This repository contains latest firmware for ESP32 peripheral module of [AIS-ADAPTER-1 Zigbee Ethernet Adapter](https://ai-speaker.com/docs/ais_zigbee_index). Firmware is opensource, so feel free to improve it by making commit to this repository.

## KEY FIRMWARE FEATURES

- Adapter mode selector throug web-interface: Zigbee-to-Ethernet and Zigbee-to-WiFI);
- Secure login through username and password;
- Zigbee2MQTT and ZHA config helper;
- Control behaviour of LED (you can disable Mode LED, Power LED through firmwares);
- DHCP or static IP address for Ethernet connection;
- ESP32 (peripheral) OTA update, ESP32  and EFR32MG21 restart;
- Switch EFR32MG21 (Zigbee) to flash mode;
- Pairing mode for adapter in router mode;
- Fully responsive web-interface based on the Bootstrap

![ais](https://github.com/sviete/AIS-ADAPTER-1/blob/main/img/ais.png)

## Installation and Configuration

Please refer to the installation and configuration articles in our [documentation](https://ai-speaker.com/docs/ais_zigbee_index).

## Compiling from source

If you made changes to the code and want to compile you own firmware, please do the following:

### You did not change web-interface appearence

- download repository;
- install Microsoft Visual Code (MVC);
- Install PlatformIO extension to MVC;
- Press "PlatformIO: Build" and wait untill firmware.bin is generated;

### You made changes to web-interface

In such case - you have to rebuild web-interface fisrt before building the firmware.

- go to the folder tools/webfilesbuilder;
- run npm install
- run npx gulp

## Contribute

You can contribute to AIS-ADAPTER-1 Firmware by:

- Providing Pull Requests (Features, Proof of Concepts or Fixes)
- Testing new released features and report issues
- Contributing missing [documentation](https://ai-speaker.com/docs/ais_zigbee_index);

## Credits

- [slzb-06-firmware](https://github.com/smlight-dev/slzb-06-firmware) This project is based on slzb-06-firmware

- slzb-06-firmware was based initially on a fork of [ZigStarGW-FW](https://github.com/xyzroe/ZigStarGW-FW) by xyzroe. Special thanks goes to xyzroe and contributors of ZigStarGW-FW.  
  
- Base code for ZigStarGW-FW was taken from [ZiGate-Ethernet](https://github.com/fairecasoimeme/ZiGate-Ethernet) and some ideas and code snippets was taken from [esp-rfid](https://github.com/esprfid/esp-rfid)

- Special thanks goes also to the authors of 3rd party libraries which are used in this project.  

## License and attribution

AIS-ADAPTER-1 firmware is licensed under GNU General Public License v3.
3rd party libraries that are used by this project are licensed under different license schemes, please check them out as well.  
Copyright (c) 2024 AI-Speaker.  
The GNU General Public License v3 ensures that if you use any part of this software in any way, your software must be released under the same license.  
