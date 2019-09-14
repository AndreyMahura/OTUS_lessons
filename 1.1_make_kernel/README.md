# OTUS_lessons
For study course of Linux Administration
###### Make a kernel linux-5.2.8 ###########
1). Install Development Tools in Linux (GNU GCC Compiler and others)
"""sudo apt-get install build-essential"""
2) Install next packets:
libncurses5-dev : Developer’s libraries for ncurses
libncursesw5-dev : Developer’s libraries for ncursesw
"""sudo apt-get install libncurses5-dev libncursesw5-dev"""

3) Copy kernel local configuration from boot to PATH with new kernel:
"""cp /boot/config* .config (Create file ".config").

4) Use command """make oldconfig""" to apply script prepare configuration on your
VM or PC and what new feaches you what to see from new kernel.
( for this you need to instal "flex", "bison".)
After all actions and your selects you will see next config file (.config)

5) Additional need to install ("libssl-dev | libelf-dev")
Now all prepared and we can install on your
Use commands:
     "make"                  --- compilete all what you need for your VM/PC.
     "make install"          --- Install
     "make modules_install"  --- Install kernel modules

