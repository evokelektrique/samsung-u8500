Firmware files for the Samsung U8500 phones
Chipsets: BCM4330 and BCM4334

The files are found in the system images in the following
locations:

- Bluetooth firmware is in /bin/BCM43nn*.hcd
- WLAN firmware is in /etc/wifi/bcm43nn_sta.bin
- WLAN settings is in /etc/wifi/nvram_net.txt

Renaming for the mainline kernel:
- The bluetooth firmwares are renamed into BCM4330B1.hcd and
  BCM4334B0.hcd because those are the names for the variants
  used by the mainline driver.
- The WLAN firmware is renamed like BCM4330B1.samsung,<modelname>.hcd
- The WLAN settings is renamed like brcmfmac4330-sdio.samsung,<modelname>.txt
  Since this is unique per phone this should ideally be copied from
  the file system.
