---
title: เปิดใช้งานตู้เซฟแนบSharePointออนไลน์ OneDriveและMicrosoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894482"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>เปิดใช้งานตู้เซฟแนบSharePointออนไลน์ OneDriveและMicrosoft Teams

1. ใช้ข้อมูลพื้นฐานของผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบความปลอดภัย ของคุณ เปิดพอร์ทัล Microsoft 365 Defender ที่ แล้วไปที่ นโยบาย <https://security.microsoft.com> **&** \> **นโยบายภัยคุกคาม** \> **ตู้เซฟ สิ่งที่แนบมา****ในส่วน** นโยบาย

   เมื่อต้องการไปยังหน้า **ตู้เซฟสิ่งที่แนบมา** <https://security.microsoft.com/safeattachmentv2> โดยตรง ให้ใช้

2. บนหน้า **ตู้เซฟสิ่งที่แนบมา** ให้คลิก **การตั้งค่า** ส่วนกลาง
3. บนเมนูOffice 365ที่ปรากฏขึ้น ให้เลือก เปิด **Microsoft Defender Office 365 SharePoint OneDrive Microsoft Teams** แล้วเลือก บันทึก

    > [!TIP]
    >
    > ให้ปฏิบัติตามขั้นตอนต่อไปนี้เพื่อป้องกันสิ่งที่แนบมาตู้เซฟสิ่งที่แนบมาSharePoint OneDrive และMicrosoft Teams:
    >
    > - เมื่อต้องการป้องกันไม่ให้ผู้ใช้ดาวน์โหลดไฟล์ที่เป็นอันตราย ให้ใช้ค่าพารามิเตอร์ `$true` *DisallowInfectedFileDownload* บน cmdlet **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** SharePoint PowerShell Online For more information see [Use SharePoint Online PowerShell to prevent users from downloading malicious files](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files).
    > - [สร้างนโยบายการแจ้งเตือนของไฟล์ที่ตรวจพบ](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

For more information, see[ตู้เซฟ Attachments for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
