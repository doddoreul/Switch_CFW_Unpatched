# Switch_CFW_Unpatched
Issues I ran into when installing CFW on a Switch V1

## Switch not entering RCM
Plug the dongle
Hold + button
Push Power button
Release + button

## Switch in RCM mode, not detected by TegraRCM
Follow this guide: https://github.com/rajkosto/TegraRcmSmash to reinstall the drivers:
### Driver setup
 1. Get your Switch into RCM mode and plug it into your Windows PC. It should show up somewhere (like Device manager) as "APX"
 2. Download and run Zadig driver installer from https://zadig.akeo.ie/
 3. From the device list, choose APX (if it's not showing up in the list, go to Options menu and check List All Devices)
 4. For the driver type, cycle the arrows until you see libusbK (v3.0.7.0) in the text box (IMPORTANT!)
 5. Click the big Install Driver button. Device manager should now show "APX" under libusbK USB Devices tree item.


## 'nosigchk'
Wrong sigpatches installed. 
Those made the trick for me: 'https://gbatemp.net/threads/sigpatches-for-atmosphere-hekate-fss0-fusee-package3.571543/page-205#post-10517797'
