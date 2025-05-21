
---

# BYD – Enable ADB & Install Apps  
Credits -> https://github.com/ahmada3mar/BYD

This repository provides a step-by-step guide on how to enable ADB (Android Debug Bridge) and Wireless ADB on BYD cars running firmware versions released after 2407.  

In the latest firmware updates, BYD has disabled standard developer tools, preventing users from installing APK files. This guide will help you bypass these restrictions and sideload apps onto your vehicle's system.  

## Enabling ADB  

1. Ensure your phone is connected to the car via **Bluetooth**.  
2. Dial the following number on the car's infotainment system:  

   ```
   *#91532547#*
   ```

3. A verification menu will appear displaying your **IMEI number**.  
4. Generate the required password:  

      - Visit the following website to 👉 [BYD Secret (online)](https://ahmada3mar.github.io/BYD/)
      
6. Enter your **IMEI number** on the website.  

   ⚠ **Make sure your car’s time is synchronized with the website’s time.**
7. Enter any one of the four codes on screen.
8. Goto test tools and enable dubg on wifi   

Once ADB is enabled, you can proceed with installing an **unlocked package installer** to allow APK sideloading.  

---

## Installing the Package Installer  

1. **Download the Package Installer APK**:  

   👉 [Download PackageInstaller.apk](https://github.com/ahmada3mar/BYD/raw/refs/heads/main/PackageInstaller.apk)  

2. Connect your PC on wifi same as pc.
3. Copy Platform-tools
4. goto Platform-tools path and open command prompt.
5. type :

```
adb connect <ipaddress of infotainment>:5555
```

6. Install the Package Installer using the following command:  

   ```
   adb install PackageInstaller.apk
   ```

Once installed, you will be able to install APK files .

```
adb install GBox-1.6.5.1-160501-20819-website.apk
```

---
