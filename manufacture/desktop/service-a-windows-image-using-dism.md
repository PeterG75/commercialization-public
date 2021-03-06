---
author: kpacquer
Description: Service a Windows Image Using DISM
ms.assetid: 7578765f-15ca-4cdd-9327-cfe42a36add2
MSHAttr: 'PreferredLib:/library/windows/hardware'
title: Service a Windows Image Using DISM
ms.author: kenpacq
ms.date: 05/02/2017
ms.topic: article


---

# Service a Windows Image Using DISM


The Deployment Image Servicing and Management (DISM) tool lets users enumerate drivers and packages, modify configuration settings, add and remove drivers without using an unattended answer file, and more. You can use DISM offline on a WIM or VHD file, or online on a running operating system.

Offline servicing allows you to modify or service a Windows® image entirely offline, without booting it first. This can reduce deployment costs because you can customize images to a degree before the operating system is deployed to the computer. In addition, if you have a stored master image that you want to make sure is always up to date, you can maintain it without booting the image.

You can also use DISM to service an image online. If you have to boot the operating system to install an application or test and validate the installation, you can boot to audit mode and add drivers and packages, or enable features and international settings.

## <span id="In_This_Section"></span><span id="in_this_section"></span><span id="IN_THIS_SECTION"></span>In This Section


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p><a href="add-and-remove-drivers-to-an-offline-windows-image.md" data-raw-source="[Add and Remove Drivers to an Offline Windows Image](add-and-remove-drivers-to-an-offline-windows-image.md)">Add and Remove Drivers to an Offline Windows Image</a></p></td>
<td align="left"><p>Add or remove drivers from an offline image using either DISM or an unattended answer file.</p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="enable-or-disable-windows-features-using-dism.md" data-raw-source="[Enable or Disable Windows Features Using DISM](enable-or-disable-windows-features-using-dism.md)">Enable or Disable Windows Features Using DISM</a></p></td>
<td align="left"><p>Enable or disable features in a Windows image using DISM. You can also remove a feature to install on-demand, and restore a previously removed feature.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="add-or-remove-packages-offline-using-dism.md" data-raw-source="[Add or Remove Packages Offline Using DISM](add-or-remove-packages-offline-using-dism.md)">Add or Remove Packages Offline Using DISM</a></p></td>
<td align="left"><p>Add or remove packages from an offline image using either DISM or an unattended answer file.</p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="add-and-remove-language-packs-offline-using-dism.md" data-raw-source="[Add and Remove Language Packs Offline Using DISM](add-and-remove-language-packs-offline-using-dism.md)">Add and Remove Language Packs Offline Using DISM</a></p></td>
<td align="left"><p>Add or remove language packs and configure international settings in an offline image using DISM.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="sideload-apps-with-dism-s14.md" data-raw-source="[Sideload Apps with DISM](sideload-apps-with-dism-s14.md)">Sideload Apps with DISM</a></p></td>
<td align="left"><p>Install line-of-business (LOB) Microsoft Store apps to a Windows image by using Windows PowerShell® or the Deployment Image Servicing and Management (DISM) platform.</p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="preinstall-apps-using-dism.md" data-raw-source="[Preinstall Apps Using DISM](preinstall-apps-using-dism.md)">Preinstall Apps Using DISM</a></p></td>
<td align="left"><p>Preinstall apps in a Windows image.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="customize-the-start-screen.md" data-raw-source="[Customize the Start Screen](customize-the-start-screen.md)">Customize the Start Screen</a></p></td>
<td align="left"><p>Customize the Start screen to include Microsoft Store apps and desktop apps that you use in your business.</p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="change-the-windows-image-to-a-higher-edition-using-dism.md" data-raw-source="[Change the Windows Image to a Higher Edition Using DISM](change-the-windows-image-to-a-higher-edition-using-dism.md)">Change the Windows Image to a Higher Edition Using DISM</a></p></td>
<td align="left"><p>Query an image to determine which edition of Windows the image is, and how to change the image to a higher edition of Windows.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="export-or-import-default-application-associations.md" data-raw-source="[Export or Import Default Application Associations](export-or-import-default-application-associations.md)">Export or Import Default Application Associations</a></p></td>
<td align="left"><p>Change the default programs associated with a file name extension or protocol in a Windows image.</p></td>
</tr>
<tr class="even">
<td align="left"><p><a href="service-a-mounted-windows-image.md" data-raw-source="[Service a Mounted Windows Image](service-a-mounted-windows-image.md)">Service a Mounted Windows Image</a></p></td>
<td align="left"><p>Use DISM to mount an image and modify it.</p></td>
</tr>
<tr class="odd">
<td align="left"><p><a href="service-an-applied-windows-image.md" data-raw-source="[Service an Applied Windows Image](service-an-applied-windows-image.md)">Service an Applied Windows Image</a></p></td>
<td align="left"><p>Use DISM to apply an image and then modify it.</p></td>
</tr>
</tbody>
</table>

 

## <span id="related_topics"></span>Related topics


[Understanding Servicing Strategies](understanding-servicing-strategies.md)

[Take Inventory of an Image or Component Using DISM](take-inventory-of-an-image-or-component-using-dism.md)

 

 






