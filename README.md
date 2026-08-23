# Wackelpudding-OS

Wackelpudding OS is an Arch-based Linux distro with support for the
[Chaotic-AUR](https://aur.chaotic.cx/).

It is early-stage software and currently maintained by a single developer.
The main goal right now is getting the Calamares installer to work the way it
does on ArcoLinux and EndeavourOS, meaning it should let you pick the packages
that get installed.

If you want to contribute or have questions, join the Discord server:
https://discord.gg/BJjWJZXbER

The live environment user is `Pro` with password `pro`. The name is leftover
from when the project was going to be called Pro OS.

## Building

Requirements: `mkarchiso`, `qemu` (for testing), and a working Arch install.

```
git clone https://github.com/Big-Smarty/Wackelpudding-OS.git
cd Wackelpudding-OS
sudo mkarchiso -v -w working-directory Wackelpudding\ OS/
```

The build takes roughly 10 to 30 minutes depending on your CPU and RAM (about
25 minutes on a Ryzen 5 3550h with 10 GB of RAM). The ISO is written to an
`out/` folder that mkarchiso creates in the directory you ran the command
from.

## Testing

From the same directory, run the finished ISO in QEMU:

```
run_archiso out/Wackelpudding_OS-xxxx.xx.xx-x86_64.iso
```

Make sure QEMU is installed.
