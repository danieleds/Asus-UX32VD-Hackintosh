# OS X on Asus UX32VD
This is a working set of kexts and configurations for running OS X on an ASUS UX32VD laptop.
Note: the original wireless card doesn't work with OS X. I've replaced it.

####System:
You can find detailed hardware information gathered from Ubuntu at [System Hardware/](System Hardware/).

 - UEFI firmware version: 214
 - CPU: Intel Core i5-3317U
 - GPU: Intel HD4000 + Nvidia GeForce GT 620M
 - Audio: ALC269VB
 - Wifi: Dell Wireless 1520 (chipset: Broadcom BCM4322 (BCM94322HM8L))
 - Bluetooth: missing. If you need it, use AzureWave AW-CE123H as WiFi card (chipset: Broadcom 20702A3 (BCM20702A0) (IDs: 0x3404, 0x13d3)).

####Status:
 - Current OS X version: El Capitan 10.11.2
 - Working:
   - CPU steps
   - Sleep
   - Audio
   - WiFi
   - Multitouch
   - FN keys
   - A lot more...
 - Not working: 
   - Card reader
   - Bluetooth (it works using an appropriate Wifi card like AzureWave AW-CE123H)
 - Not working (not tested properly):
   - HDMI
   - iMessage
   - Handoff
   - Instant Hotspot
   - Hibernation
   - Nvidia GeForce GT 620M

####What is inside this repo:
 - A working DSDT: [DSDT-SSDT/](DSDT-SSDT/).
 - Instructions on how the DSDT has been made, in case you want to patch your own: [DSDT-SSDT-src/](DSDT-SSDT-src/).

<!--
- [Clover](http://sourceforge.net/projects/cloverefiboot/) config.plist and drivers
- DSDT and SSDT (SSDT generated with [ssdtPRgen](https://github.com/Piker-Alpha/ssdtPRGen.sh) v13.2: "$ ./ssdtPRgen.sh -x 1 -lfm 900")
- Various kexts:
	- [ACPIBatteryManager](https://bitbucket.org/RehabMan/os-x-acpi-battery-driver)
	- [ApplePS2SmartTouchPad](http://forum.osxlatitude.com/index.php?/topic/1948-elan-focaltech-and-synaptics-smart-touchpad-driver-mac-os-x/): touchpad and keyboard (this is set to ISO and italian keyboard layout)
	- [AsusNBFnKeys](http://forum.osxlatitude.com/index.php?/topic/1968-fn-hotkey-and-als-sensor-driver-for-asus-notebooks/)
	- [Brcm\*](https://bitbucket.org/RehabMan/os-x-brcmpatchram): bluetooth
	- DummyHDA: to use Apple's audio driver
	- [EAPDFix](http://forum.osxlatitude.com/index.php?/topic/3084-eapdjack-sense-fix-no-audiojack-sense-issue-after-sleep/): to fix audio after sleep
	- [FakePCIID\*](https://bitbucket.org/RehabMan/os-x-fake-pci-id): to make wifi and USB 3.0 work
	- [FakeSMC](http://www.hwsensors.com): essential to boot OS X; no plugins installed
	- [IntelBacklight](https://bitbucket.org/RehabMan/os-x-intel-backlight): for display backlight
-->
