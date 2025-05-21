
---
---
### **User Responsibility & Disclaimer**

This guide outlines how to enable advanced features on your BYD's infotainment system. While we strive for accuracy, it's vital to understand the implications of these actions.

**You are solely responsible for any consequences** that may occur after enabling ADB and installing applications not officially sanctioned by BYD. This includes, but is not limited to:

* **Potential voiding of your vehicle's warranty.**
* **System malfunctions or bricking of the infotainment unit.**
* **Security vulnerabilities and data privacy risks.**
* **Performance issues or instability.**

We provide this information as a guide, but **we offer no guarantees and accept no liability** for any outcomes resulting from its use. If you are not comfortable with these risks, please do not proceed.
---
# BYD – Enable ADB & Install Apps  
Credits -> https://github.com/ahmada3mar/BYD

!Disclamer : 
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
   **Download**  
👉 [Platform tools](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)
3. Extract in a folder Platform-tools
4. goto Platform-tools , make sure you see all files in the path and open command prompt.
5. type :

```
adb connect <ipaddress of infotainment>:5555
```

6. Install the Package Installer using the following command:  

   ```
   adb install PackageInstaller.apk
   ```

Once installed, you will be able to install APK files .

**Donwload Gbox**
👉 [GBOX](https://agile-files.gboxlab.com/GBox-1.6.5.1-160501-20819-website.apk)
```
adb install GBox-1.6.5.1-160501-20819-website.apk
```

---
