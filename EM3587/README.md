# zigbee-firmware
## ZigBee Development Firmware

_Note: Generally only 57k6 Baud is supported on EM358x boards - however 115k2 has been used with some success._

## EM3587 Long Range Versions
__NCP_USW_EM3587-LR_678-115k2__
* NCP - Silabs NCP
* USW - Uart interface, Software Flow Control 
* EM3587 - Long Range EM3587 Dev0680 Based Device PB1=TXD, PB2=RXD
* 678 - EmberZNet Version (EZSP V8!)
* 115k2 - Baud Rate

__BTL_STD_EM3587.s37__
* Standalone uart xmodem bootloader for EM3587