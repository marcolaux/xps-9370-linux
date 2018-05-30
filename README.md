# xps-9370-linux
fix things on the Dell XPS 13 9370 on GNU/Linux

- ~~This should include the right Bluetooth firmware from the windows drivers to prevent the problem that the Bluetooth device sometimes disappears after supsend.~~
  this was useless
  
- added the default/grub file as a reference for the kernel parameters
  - wich enables the 9370 to go into deep sleep mode
  - if the btusb-parameter is for any use because of the bluetooth gone after suspend problem - we'll see

- Made a script that disables wakeup on the PCI 00:14.0 device (had a problem with automatic wakeups when connected to stuff via USB-C)
  - the device is "00:14.0 USB controller: Intel Corporation Sunrise Point-LP USB 3.0 xHCI Controller (rev 21)"
  - enable the 9370boot.service for the script to run on boot
