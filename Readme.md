Easy way to get Root access on Android Simulator
--
1 - Download this repo

2 - Copy su and Superuser.apk files into  <YOUR_SDK_INSTALL_DIR_PATH>/platform-tools/

3 - go to the sdk location <YOUR_SDK_INSTALL_DIR_PATH>/platform-tools/ and execute few commands.
  
  adb remount

  adb push su /system/xbin/su

  adb shell chmod 06755 /system

  adb shell chmod 06755 /system/xbin/su

  adb install Superuser.apk
 

Now you can execute

  adb shell

  su

