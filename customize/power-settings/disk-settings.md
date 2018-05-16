---
title: Disk settings
description: Settings in this subgroup control the power management of disk devices.
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 2C6AA970-C955-4690-BA89-8CBF5EA51ED7
author: alhopper-msft
ms.author: alhopper
ms.date: 10/05/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-oem
---

# Disk settings


Settings in this subgroup control the power management of disk devices.

## <span id="Subgroup__GUID__aliases__and_setting_visibility"></span><span id="subgroup__guid__aliases__and_setting_visibility"></span><span id="SUBGROUP__GUID__ALIASES__AND_SETTING_VISIBILITY"></span>Subgroup, GUID, aliases, and setting visibility


-   **Subgroup:** Disk settings

-   **GUID:** 0012ee47-9041-4b5d-9b77-535fba8b1442

-   **Windows provisioning path:** `Common\Power\Policy\Settings\Disk`

-   **PowerCfg alias:** `SUB_DISK`

-   **Hidden setting:** Yes

## <span id="in_this_section"></span>In this section


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Topic</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>[Disk burst ignore time](disk-settings-disk-burst-ignore-time.md)</p></td>
<td><p>Specifies the period of inactivity to ignore when attempting to aggressively power down the disk.</p></td>
</tr>
<tr class="even">
<td><p>[Disk idle timeout](disk-settings-disk-idle-timeout.md)</p></td>
<td><p>Specifies the period of inactivity before the disk is automatically powered down.</p></td>
</tr>
<tr class="odd">
<td><p>[Link power management mode - adaptive](disk-settings-link-power-management-mode---adaptive.md)</p></td>
<td><p>Specifies the period of AHCI link idle time before the link is put into a slumber state when Host-Initiated Power Management (HIPM) or Device-Initiated Power Management (DIPM) is enabled.</p></td>
</tr>
<tr class="even">
<td><p>[Link power management mode - HIPM/DIPM](disk-settings-link-power-management-mode---hipm-dipm.md)</p></td>
<td><p>Configures the link power management mode for disk and storage devices that are attached to the system through an AHCI interface.</p></td>
</tr>
</tbody>
</table>
