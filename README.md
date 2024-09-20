<div align="center">

  <img src="https://user-images.githubusercontent.com/62047147/195847997-97553030-3b79-4643-9f2c-1f04bba6b989.png" alt="logo" width="100" height="auto" />
  
  <h1> HuginsRage </h1>
  <p> DIY USB Rubber Ducky based on RP2040 </p>
  
</div>

<br />  

## 🌟 About the Project
HuginsRage enables anyone to build a powerful USB keystroke injection tool with simple hardware. It’s inspired by the original USB Rubber Ducky but allows for more flexibility by using a customizable microcontroller (RP2040) and an SD card for payload storage. This makes it ideal for both educational purposes and professional use in security assessments.

<div align="center"> 
  <img src="---" alt="screenshot" width="Auto" height="Auto" />
</div>


## 🎯 Features, Software and Hardware
### Features
- **SD Card Hot-Swap**: Detects SD card insertion even when powered.
- **Keystroke Injection**: Execute commands stored in a `script.txt` file.
- **LED Indicators**:
  - Blinks every second when no SD card is present.
  - Blinks every 2 seconds when no script is found.
  - Blinks on each keystroke during script execution.
- **Supports Rubber Ducky-style Scripts**: Commands like `STRING`, `DELAY`, and special keypresses.


### Software Requirements
- **Arduino IDE**: Version 1.8 or higher
- **Board Plug-In**: Arduino-Pico, from Earle F. Phillhower (https://github.com/earlephilhower/arduino-pico)
- **Libraries**:
  - SD
  - SPI
  - Keyboard

### Hardware Requirements
- **Microcontroller**: RP2040
- **MicroSD card**: Formatted as FAT16/32
- **LED**: Connected to indicate status
- **SD Card Module**: For reading scripts


## 🔌 Schematic
The detailed schematic of the HuginsRage setup can be found [here](https://cifertech.net/HuginsRage-diy-usb-rubber-ducky-for-ethical-hacking/). This will guide you in wiring the SD card module and LED to your RP2040.

1. Connect the SD card module to the RP2040 using these pins:
   - **CS** -> Pin 4
   - **MOSI** -> Pin 11
   - **MISO** -> Pin 12
   - **SCK** -> Pin 13
2. Connect the status LED:
   - **Anode** -> Pin 9
   - **Cathode** -> Ground
  
<div align="center"> 
  <img src="https://github.com/user-attachments/assets/abd5b46d-fdbf-49c9-b2a4-dd321f4ae481" alt="screenshot" width="Auto" height="Auto" />
</div>


## ⚠ Future Changes
Future updates may include:
- **Improved Error Handling**: More detailed feedback on SD card or file issues.
- **Multiple Script Files**: Ability to load and execute multiple scripts.
- **Additional Commands**: Expanding the supported command set for more advanced payloads.


<!-- License -->
## :warning: License

Distributed under the MIT License. See LICENSE.txt for more information.


<!-- Contact -->
## :handshake: Contact

▶ Support me on Patreon [patreon.com/cifertech](https://www.patreon.com/cifertech)

CiferTech - [@twitter](https://twitter.com/techcifer) - CiferTech@gmali.com

Project Link: [https://github.com/cifertech/HuginsRage](https://github.com/cifertech/HuginsRage)


