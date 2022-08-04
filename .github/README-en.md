# OC-DELL-OptiPlex7040MICRO
Opencore EFI for Dell OptiPlex 7040 Micro

## Hardware
| Model            | Dell OptiPlex 7040 Micro    |
|------------------|-----------------------------|
| CPU              | i5-6500T                    |
| Intel Graphic    | HD530                       |
| Memory           | DDR4 2133 8+8               |
| SSD              | Samsung 960EVO 250GB (PCIE) |
| Audio            | Realtek ALC255              |
| WLAN + Bluetooth | Intel AC8260                |
| Ethernet         | Intel I219-LM               |

## System available

MacOS Monterey Version 12.4 **12.5**

If you use Bigsur, please modify the file yourself (mainly just change some WiFi and Bluetooth related settings).

## Opencore version and kexts

- Opencore 0.7.8 **0.8.2**
- The latest version of BlueToolFixup is not available on my machine, use version 2.6.2 instead.

## Statements

- Please unlock CGF lock and adjust DVMT, tutorial can refer to this [link](https://github.com/optiplex-osx/Dell-OptiPlex-7040-Clover-EFI%0A).
- I personally do not use OSX and Windows together, if it causes some problems for the Windows, please solve it by yourself.
- I do not use the HDMI interface, please customize it if you need to use it.
- Please update the serial number before use.

## Conditions

- CPU: Frequency adjustment and temperature work well.
- Audio: Headphones and built-in speakers work fine.
- Intel Graphic：DP output work fine.
- Bluetooth and WLAN: Work fine, but AirDrop and Sidecar cannot be used due to the limitation of Intel network card. But if you connect your iPad with a wire, you can use Sidecar.
- USB：
    - USB3 and USB2 devices work fine.
- SSD：
    - Because the hard disk I am using does not support Trim well, so I turn off this function.

## Credits

- Apple
- [@Acidanthera](https://github.com/acidanthera)
- [@daliansky](https://github.com/daliansky)
- And other unlisted developers.

