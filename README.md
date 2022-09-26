<h1 align="center">
GameConsole_ESP32
</h1>

## Introduction
This project is one of the work in Makereal Labs, NYCU. The first game console is equipped with Arduino Nano. Although there are many libraries can be used in Arduino, the memory and speed for Nano is too small for games computing a lot. This version of game console uses ESP32; thus has much more functions and memory. The ping-pong game inside can be played by two people or played with computer.

### Set up environment for ESP32 & TFT_espi
(Almost same for Windows and Mac)
1. In Arduino IDE: File -> preference -> extra url -> https://dl.espressif.com/dl/package_esp32_index.json
2. Tool -> board manager -> search "esp32" -> install esp32 (1.0.6 version)
3. Tool -> board -> choose "ESP32 Arduino" -> choose "ESP32 Dev Module"
4. Tool -> function manager -> search "TFT_espi" and install it
5. Find user_setup.h in documents in PC and replace code with user_setup.h in this GitHub

### user_setup.h
Record the specific pinMode in game console, which is different from the default settings in the library for TFT_eSPI

### ping-pong_canwin.ino
This version is a more friendly one. The speed of computer in single mode has been randomly made slowly and the final points for winning is six

### ping-pong_neverwin.ino
The score to win of this version is 11 and the speed of computer is too fast to win for players 
