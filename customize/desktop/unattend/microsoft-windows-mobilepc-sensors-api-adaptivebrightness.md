---
title: AdaptiveBrightness
description: AdaptiveBrightness
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: c60042e8-652f-4f9f-9cc0-2e93c17022a6
ms.mktglfcycl: deploy
ms.sitesec: msdn
author: alhopper-msft
ms.author: alhopper
ms.date: 05/02/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---
# AdaptiveBrightness

`AdaptiveBrightness` contains settings related to adaptive brightness.

Adaptive brightness changes the brightness of a monitor or display based on the ambient light.

## Child Elements

| Setting                 | Description                                                                           |
|:------------------------|:--------------------------------------------------------------------------------------|
| [ALRPoints](microsoft-windows-mobilepc-sensors-api-adaptivebrightness-alrpoints.md) | Specifies the ambient light response (ALR) curve data. |
| [DisplayResponseInterval](microsoft-windows-mobilepc-sensors-api-adaptivebrightness-displayresponseinterval.md) | Specifies the minimum time, in milliseconds, between changes in display brightness due to lighting conditions. |
| [IlluminanceChangeSensitivity](microsoft-windows-mobilepc-sensors-api-adaptivebrightness-illuminancechangesensitivity.md) | Specifies the percentage change in illuminance (lux) required to cause a change in display brightness. Specified in percentage change since the last change in display brightness. |

## Valid Passes

specialize

## Parent Hierarchy

[Microsoft-Windows-MobilePC-Sensors-API](microsoft-windows-mobilepc-sensors-api.md) | **AdaptiveBrightness**

## Applies To

For the list of the supported Windows editions and architectures that this component supports, see [microsoft-windows-mobilepc-sensors-api-](microsoft-windows-mobilepc-sensors-api.md).

## XML Example

The following sample XML output shows how to set adaptive brightness:

```XML
<ALRPoints>000000000a0000000a00000028000000280000005000000044</ALRPoints>
<DisplayResponseInterval>60000</DisplayResponseInterval>
<IlluminanceChangeSensitivity>20</IlluminanceChangeSensitivity>
```

## Related topics

[Microsoft-Windows-MobilePC-Sensors-API](microsoft-windows-mobilepc-sensors-api.md)
