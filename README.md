# zigbee-firmware

## Zigbee Development Firmware

### Usage

* Make sure device drivers for USB-to-UART bridge/conveter is already installed if required.
* Stop any application/service/integration that is connected to the serial port of the adapter.
* Backup NVRAM with [bellows CLI tools](https://github.com/zigpy/bellows) (Python 3 script).
* Install [Elelabs Firmware Update Utility](https://github.com/Elelabs/elelabs-zigbee-ezsp-utility) (Python 3 script).
  * Can optionally be used it via [walthowd's Docker image environment](https://github.com/walthowd/husbzb-firmware/).
* Download correct firmware image for your chip.
* Use command `python Elelabs_EzspFwUtility.py flash -p /dev/select/correct/tty-device -f 'path/to/firmware.gbl'`

### Versions

__Folders containing different versions of bootloader and NCP firmware.__

* EFR32 Series 1
* EFR32 Series 2
  * EFR32MG21A020F1024 <sup>C
* EFR32MG2x-768k <sup>B  
* EFR32MG22 <sup>B
* EM357     <sup>A
* EM3581    <sup>A
* EM3585    <sup>A
* EM3587    <sup>A
* EM3588    <sup>A
* GFR8LE
* MG1B232
* Sonoff-ZBBridge <sup>B

__Notes__
+ A -> Updated to EmberZNet 6.7.10
+ B -> Updated to EmberZNet 6.10.3
+ C -> Added EmberZNet 7.0.1

__Folders containing legacy firmware for older Ember/Silabs chips.__
* EM250
  
