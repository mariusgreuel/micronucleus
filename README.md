# Micronucleus - ATTiny USB bootloader with a strong emphasis on bootloader compactness

This is a fork of the [Micronucleus bootloader](https://github.com/micronucleus/micronucleus).

The goal of this fork is to add support for WinUSB to eliminate the need for third-party USB drivers in Windows, such as libusb0.

In this firmware, a [Microsoft OS feature descriptor](https://docs.microsoft.com/en-us/windows-hardware/drivers/usbcon/microsoft-defined-usb-descriptors) and WinUSB compatibility descriptor was added. When a USB device with this firmware is plugged in, Windows will automatically load the built-in WinUSB driver.

In order to use the Micronucleus bootloader with WinUSB support, you also need tools that support WinUSB, such as [AVRDUDE for Windows](https://github.com/mariusgreuel/avrdude).

The original readme.txt can be found here: [Readme.txt](Readme.txt)
