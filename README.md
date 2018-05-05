# xps-9370-linux
fix things on the Dell XPS 13 9370 on GNU/Linux

- This should include the right Bluetooth firmware from the windows drivers to prevent the problem that the Bluetooth device sometimes disappears after supsend.

- Made a script that disables wakeup on the PCI 00:14.0 device (had a problem with automatic wakeups when connected to stuff via USB-C)
  - the device is "00:14.0 USB controller: Intel Corporation Sunrise Point-LP USB 3.0 xHCI Controller (rev 21)"
  - enable the 9370boot.service for the script to run on boot
