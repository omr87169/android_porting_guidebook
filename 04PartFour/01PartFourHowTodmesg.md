How to use dmesg to examine your hardware
=========================================
Sometimes you will need to import a repository or object file which applies to a
specific piece of hardware on your device, and sometimes, you won't even have 
access to the name of that piece of hardware. 

In this case, the closest to a universal means to discern what this hardware is
to use [dmesg](https://en.wikipedia.org/wiki/Dmesg), the driver messaging 
system. In order to do this you will need to connect to the device via "adb 
shell" or use the Terminal Emulator or ConnectBot App, both of which are 
available in F-Droid and the Google Play Store.

Installing a Terminal Emulator
------------------------------
To use dmesg, you will need to have access to a Terminal Emulator on the device.
If you want, you can use "adb shell", but if not you can install a Terminal
Emulator on the device. There are two Free Software options available.

###Which one?
Well it depends. It's totally possible to use dmesg with either of them, and
there is not much difference between the two of them. The short of it is that if
you only want to work on the device, Android Terminal Emulator is the one for
you. If you want advanced features or the ability to ssh to another machine,
then you should use ConnectBot.

####Android Terminal Emulator
[Android Terminal Emulator](https://f-droid.org/repository/browse/?fdfilter=terminal&fdid=jackpal.androidterm) is an easy to use Terminal Emulator
available from F-Droid, as an APK, and from the Google Play store. It is
intended to provide a terminal for your device, on your device.

####ConnectBot Android Shell
[ConnectBot Android Shell](https://f-droid.org/repository/browse/?fdid=org.connectbot)
is a terminal emulator and secure shell client. It can be run in terminal
emulator mode, or it can be used to connect via ssh to a remote machine. It can
also be used to connect to a GNU/Linux chroot and launch some X applications if
they are supported on your device.

Working in the Terminal Emulator
--------------------------------


###Step-by-Step

####Stop the hardware in question

####

####

Further Citations
-----------------
[How do I find out what Wi-Fi Chipset my phone has](https://android.stackexchange.com/questions/13548/how-do-i-find-out-what-wifi-chipset-my-phone-has) Android Stack Exchange, GAThrawn, Gili

