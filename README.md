# xps-9370-linux
fix things on the Dell XPS 13 9370 on GNU/Linux

EDIT: I don't update this anymore. Dell had a year to fix the "missing bluetooth after suspend" issue (https://www.dell.com/community/Linux-Developer-Systems/XPS-13-9370-no-bluetooth-after-suspend) without success. I felt like a beta tester for this product and have enough now. It's not acceptable to fully shutdown the mashine just to get bluetooth back so I can use my keyboard and mouse again when I have multiple workspaces with tons of windows open. 

Dell please do you users a favour and test those things under Linux and give a guarantee on it that you support it. When I called the support they told me: "It's your fault - you installed an unsupported operating system". Great, why buying the developer edition in the first place?

I'm done with this thing.

- added the default/grub file as a reference for the kernel parameters
  - wich enables the 9370 to go into deep sleep mode

- made a script and service that detects my eGPU NVIDIA setup on boot

- my lenovo_fix.conf for
  https://github.com/erpalma/lenovo-throttling-fix
  
- powertop autotune service that starts on boot
