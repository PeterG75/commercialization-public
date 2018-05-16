---
title: Common write filter exclusions
description: Common write filter exclusions
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: cbae7b49-23b0-4232-91d7-b61b2adc8cd5
author: alhopper-msft
ms.author: alhopper
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---
# Common write filter exclusions

Some services and features write information to a device’s persistent volume, and expect that information to be present across device restarts. You may need to configure your write filter to allow for specific file and registry exclusions in order for these services and features to work correctly.

This topic lists registry and file exclusions that can help enable some common services and features to work correctly when write filters are enabled.

## Customer Experience Improvement Program (CEIP)

When you choose to participate in the CEIP, your computer or device automatically sends information to Microsoft about how you use certain products. Information from your computer or device is combined with other CEIP data to help Microsoft solve problems and to improve the products and features customers use most often.

CEIP data is stored in files that have a .sqm file name extension. To make sure that the CEIP data in the .sqm files is available on a device that has write filters enabled, you can add file and folder exclusions for the .sqm files and folders.

To locate the .sqm files and folders on your device, search for .sqm files by using File Explorer. Alternately, at a command prompt with administrator rights at the root of the drive, type the following command to obtain a list of .sqm files on the device:

```powershell
dir *.sqm /s
```

Add file and folder exclusions as required for any .sqm files located on your device.

Add registry exclusions for the following registry keys:

* **HKEY\_LOCAL\_MACHINE\\Software\\Policies\\Microsoft\\SQMClient\\Windows\\CEIPEnable**

* **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\SQMClient\\Windows\\CEIPEnable**

* **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\SQMClient\\UploadDisableFlag**

## Background Intelligent Transfer Service (BITS)

Background Intelligent Transfer Service (BITS) downloads or uploads files between a client and server and provides progress information related to the transfers.

Add file exclusions for the following folders and files:

* *% ALLUSERSPROFILE%*\\Microsoft\\Network\\Downloader

Add registry exclusions for the following registry keys:

* **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\Windows\\CurrentVersion\\BITS\\StateIndex**

## Windows Explorer

When write filters are active and you attempt to delete an excluded file or folder in Windows Explorer, the system attempts to move the file or folder to the Recycle Bin. This causes an error, because you cannot move files that are not filtered to a location that is write filter protected.

To work around this, you can disable the Recycle Bin. Alternatively, the user can press Ctrl+Shift and then left-click on the file to directly delete the excluded file, bypassing the Recycle Bin, or the user can delete the excluded file directly from a command prompt.

## Networks

When you use write filters on your device, you can add file and registry exclusions to enable your device to join wired and wireless networks. The following file and registry exclusions may be required on your device.

Client Group Policy Object (GPO) registry keys:

* Wireless: **HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Policies\\Microsoft\\Windows\\Wireless\\GPTWirelessPolicy**
* Wired: **HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Policies\\Microsoft\\Windows\\WiredL2\\GP\_Policy**

GPO policy files:

* Wireless: **C:\\Windows\\wlansvc\\Policies**
* Wired: **C:\\Windows\\dot2svc\\Policies**

Interface profile registry keys:

* Wireless: **HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Microsoft\\wlansvc**
* Wired: **HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Microsoft\\dot3svc**

Interface policy file:

* Wireless: **C:\\ProgramData\\Microsoft\\wlansvc\\Profiles\\Interfaces\\{***&lt;Interface GUID&gt;***}\\{***&lt;Profile GUID&gt;***}.xml**
* Wired: **C:\\ProgramData\\Microsoft\\dot3svc\\Profiles\\Interfaces\\{***&lt;Interface GUID&gt;***}\\{***&lt;Profile GUID&gt;***}.xml**

Services registry keys:

* Wireless: **HKEY\_LOCAL\_MACHINE\\SYSTEM\\CurrentControlSet\\services\\Wlansvc**
* Wireless: **HKEY\_LOCAL\_MACHINE\\SYSTEM\\CurrentControlSet\\services\\WwanSvc**
* Wired: **HKEY\_LOCAL\_MACHINE\\SYSTEM\\CurrentControlSet\\services\\dot3svc**

## Daylight saving time (DST)


You can add the following registry exclusions to persist daylight saving time (DST) settings on your device.

* **HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Microsoft\\Windows NT\\CurrentVersion\\Time Zones**

* **HKEY\_LOCAL\_MACHINE\\SYSTEM\\CurrentControlSet\\Control\\TimeZoneInformation**

## Related topics

[Unified Write Filter](unified-write-filter.md)

[Service UWF-protected devices](service-uwf-protected-devices.md)

[Unified Write Filter WMI provider reference](uwf-wmi-provider-reference.md)
