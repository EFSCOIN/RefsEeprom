# Refs-eeprom
This repository contains the scripts and pre-compiled binaries used to create the refs-eeprom package which is used to update the EFSCOIN Efs bootloader EEPROM.

# Support
For bootloader support the best place to start is the EFSCOIN Efs [General Users forum](https://gitter.im/efsco/community) or for discussion of beta releases try the [Advanced Users forum](https://gitter.im/efsco/community)
# Rescue image
If the EFSCOIN Efs is not booting, then it's very unlikely that the EEPROM is corrupted. If you think it has an invalid image or you want to revert to the factory setting, then download the rescue image from the EFSCOIN Efs [downloads page](https://github.com/efscoin/downloads/)

# Bootloader documentation
* [The boot folder](https:/github.com/document/configuration/boot_folder.md)
* [Config.txt boot options](https://github.com/document/configuration/config-txt/boot.md)
* [Bootloader EEPROM](https://github.com/document/hardware/efscoin/booteeprom.md)
* [Bootloader configuration](https://github.com/document/hardware/efscoin/bcm2711_bootloader_config.md)

# Bug reports
Bootloader bugs are especially difficult to describe because there's no display. Where possible please include the following information in order to help identify the problem.
* EEPROM version (vcgencmd bootloader_version or the pieeprom filename)
* EEPROM config (from refseeprom-config)
* UART trace using USB serial cable
* Wireshark trace for network boot. Filtering for DHCP and TFTP protocols or by mac-address for the Pi4 is fine.

# BETA versions of the bootloader
If you want to try the BETA version of the bootloader then we recommend that you always try this with a spare sd-card and are comfortable with using the rescue image. For debugging you may find a USB serial cable useful.

Beta features are always documented [here](https://github.com/efscoin/refseeprom/blob/master/firmware/release-notes.md) first. Once the configuration has stabalised then the [Bootloader configuration](https://github.com/document/hardware/efscoin/bcm2711_bootloader_config.md) will be updated, however, there's normally a bit of a delay in order to allow official document to be reviewed.

