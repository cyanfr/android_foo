01. Download and install Google’s Android Studio.  Accept defaults.</br>
02. Start Android Studio and check that "Google USB Driver" is checked in settings.  Check it if not.</br>
    more instruction on that here:  https://developer.android.com/studio/run/win-usb.html
03. Reboot PC.
04. Download the correct Android OTA Update for your Pixel device to your PC.<br/>
    Check your about device's settings > about device > build number screen for your current version.<br/>
    OTAs are available here:  https://developers.google.com/android/nexus/ota#instructions<br/>
    After download, rename the zip file to npixelota.zip.
05. Enable Developer Mode on your Pixel device.
06. Enable USB Debugging Mode on your Pixel device.
07. Download and install either just the Android SDK or Android Studio and install.<br/>
    https://developer.android.com/sdk/installing/index.html
08. Open a command window and type:<br/>
    ```
    adb devices
    ```
09. Connect your Pixel phone with a USB cable.
10. Watch your phone for the prompt to "Allow USB Debugging?"<br/>
    Check "Always allow..." and hit "OK".
11. In the command window, type adb devices again and you should see your phone listed.
12. Still in the command window, type:
    ```
    adb reboot recovery
    ```
13. On the screen with the android on its back and the exclamation point in a red triangle, hold power and then press vol up once.
14. Now on the recovery screen, press vol down until "Apply Update from ADB" is highlighted.<br/>
    Press power once.
15. Reconnect your phone via the USB cable.
16. In Windows Explorer, go to one directory below the directory to which you downloaded the OTA file.<br/>
    Hold the shift key.<br/>
    Right click on the directory with the zip file.<br/>
    Select "Open command window here".
17. Type the following into the new command window:<br/>
    ```
    adb sideload pixelota.zip
    ```
    ...and press enter on your computer.
18. Wait for the OTA to copy to the phone and update it.
19. When update is complete, the Recovery choices will come back with the reboot choice highlighted.<br/>
    Disconnect phone from USB cable.<br/>
    Press power once to reboot.
20. The first boot after update will take a while.
