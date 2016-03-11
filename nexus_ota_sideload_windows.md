01. Download and install Google’s USB Drivers.\n
    https://developer.android.com/sdk/win-usb.html
02. Reboot PC.
03. Download the correct Android OTA Update for your Nexus device to your PC.
    Check your about device's settings > about device > build number screen for your current version.
    After download, rename the zip file to nexusota.zip.
04. Enable Developer Mode on your Nexus device.
05. Enable USB Debugging Mode on your Nexus device.
06. Download and install either just the Android SDK or Android Studio and install.
    https://developer.android.com/sdk/installing/index.html
07. Open a command window and type
    adb devices
08. Connect your Nexus phone with a USB cable.
09. Watch your phone for the prompt to "Allow USB Debugging?"
    Check "Always allow..." and hit "OK".
10. In the command window, type adb devices again and you should see your phone listed.
11. Disconnect phone from USB cable.
12. Boot your Nexus into Fastboot Mode.
    Power off.
    Power on by holding power + vol up + vol down all at the same time.
13. Switch to recovery mode from fastboot.
    Vol down twice to highligh Recovery Mode.  Then press power once.
14. On the screen with the android on its back and the exclamation point in a red triangle, hold power and then press vol up once.
15. Now on the recovery screen, press vol down until "Apply Update from ADB" is highlighted.
    Press power once.
16. Reconnect your phone via the USB cable.
17. In Windows Explorer, go to one directory below the directory to which you downloaded the OTA file.
    Hold the shift key.
    Right click on the directory with the zip file.
    Select "Open command window here".
18. Type the following into the new command window:
    adb sideload nexusota.zip
    ...and press enter on your computer.
19. Wait for the OTA to copy to the phone and update it.
20. When update is complete, the Recovery choices will come back with the reboot choice highlighted.
    Disconnect phone from USB cable.
    Press power once to reboot.
21. The first boot after update will take a while.
