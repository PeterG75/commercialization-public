---
title: WindowsShiftDown
description: Blocks the Windows logo key+Shift+Down Arrow key combination used to minimize the active window.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 8236E25D-11E9-4222-BED7-BE2041E858AA
author: themar-msft
ms.author: themar
ms.date: 05/02/2017
ms.topic: article


---

# WindowsShiftDown


Blocks the Windows logo key+Shift+Down Arrow key combination used to minimize the active window.

## Type


String

## Values


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Value</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><em>Allowed</em></p></td>
<td><p>The Windows logo key+Shift+Down arrow key combination is not blocked.</p>
<p>This is the default value.</p></td>
</tr>
<tr class="even">
<td><p><em>Blocked</em></p></td>
<td><p>The Windows logo key+Shift+Down arrow key combination is blocked.</p></td>
</tr>
</tbody>
</table>

 

## Parent Hierarchy


[Microsoft-Windows-Embedded-KeyboardFilterService](microsoft-windows-embedded-keyboardfilterservice.md) | **WindowsShiftDown**

## Valid Configuration Passes


offlineServicing

## Applies To


For a list of the Windows editions and architectures that this component supports, see [Microsoft-Windows-Embedded-KeyboardFilterService](microsoft-windows-embedded-keyboardfilterservice.md).

## XML example


```
<settings pass="offlineServicing">
    <component name="Microsoft-Windows-Embedded-KeyboardFilterService" processorArchitecture="amd64" publicKeyToken="31bf3856ad364e35" language="neutral" versionScope="NonSxS" xmlns:wcm="http://schemas.microsoft.com/WMIConfig/2002/State" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
        <WindowsShiftDown>Blocked</WindowsShiftDown>
    </component>
</settings>
```

 

 






