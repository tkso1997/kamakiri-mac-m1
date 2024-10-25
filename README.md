The modification in this fork allowed me to run gpt-fix.sh on macOS on a mac-m1 (no live Linux required). 

Steps to get it running under macOS 15.0.1 - assuming you have a running python3 environment:
1. Generate a virtual python environment:
   - python3 -m venv .venv
   - source .venv/bin/activate
2. install pyserial and pyusb
   - pip3 install pyusb
   - pip3 install pyserial
3. get the necessary binary files and place them in the right folders (gpt-mantis.bin etc. - google is your friend)
3. connect your FireTV-4k Mantis device to your usb port and instantaneously run gpt-fix
   - sh gpt-fix.sh

Important information:
bootrom-step.sh was not tested and might not work. The device used was already unlocked but got stuck boot-loop after I messed up some things. Using gtp-fix.sh allowed me to recover it.
