# Setting up the Meta Quest 2 PC and the Oculus Developer Hub (OHD)

### Preexisting requierments:

Installed Oculus Developer Hub (OHD):
>For Windows: https://developer.oculus.com/downloads/package/oculus-developer-hub-win

>For Mac: https://developer.oculus.com/downloads/package/oculus-developer-hub-mac

An Meta Quest 2 in Developer Mode: 
>https://developer.oculus.com/documentation/native/android/mobile-device-setup/

***
### Preparing the Meta quest 2 and the ODH (one time only):
1.	Connect the Meta Quest 2 to your PC and copy the folder "hls.js" to the internal storage of the Headset.  
(next to the download and oculus folder)

2.	Create in OHD this custom command: 
```adb 
adb -s _ODH_CONNECTED_DEVICE_SERIAL_ID_ shell am start \-n com.oculus.os.vrbrowserlauncher/.MainActivity \-a android.intent.action.VIEW -d 'file:///storage/emulated/0/hls.js/index.html' 
```

***
### Accessing the Website with the livestream on the Meta Quest 2:
1.	Connect the Meta Quest 2 to your PC and run in OHD the created custom command.
2.	Dissconnect and put on the Meta Quest 2.
