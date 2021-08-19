# Wackelpudding-OS
Wackelpudding OS is an Arch based linux distro with support for chaotic-aur.
Currently I'm the only developer working on it since... yesterday lol.
My plans currently are to get the calamares installer working in a way like with arco and endeavour (as in having it install chosen packages).
If you wanna contribute to this project join this discord server: https://discord.gg/BJjWJZXbER

The username is "Pro" and the password is "pro" (originally this was meant to be called Pro OS)

You can also join this server if you have questions or problems with it or whatever

To build Wackelpudding OS, run this:

git clone https://github.com/Big-Smarty/Wackelpudding-OS.git

cd Wackelpudding-OS

sudo mkarchiso -v -w working-directory Wackelpudding\ OS/

This will take like 10 to 30 minutes depending on your CPU and the amount of RAM you have (on my system [10 GB RAM Ryzen 5 3550h] it takes like 25 minutes).
The ISO will be in an "out/" folder which was generated automatically in the directory you were in when you ran the command.

To then run the completed ISO, given you're in the same directory as when running the command from before, run this:

run_archiso out/Wackepludding-OS-xxxx.xx.xx-x86_64.iso

(make sure to have qemu installed)

