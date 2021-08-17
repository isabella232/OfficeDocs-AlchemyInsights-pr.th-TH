---
title: เปิดใช้งาน Microsoft Defender Office 365 for SharePoint Online, OneDrive และ Microsoft Teams
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
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058885"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>เปิดใช้งาน Microsoft Defender Office 365 for SharePoint Online, OneDrive และ Microsoft Teams

1. ใช้ข้อมูลรับรองความถูกต้องของผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบความปลอดภัย ของคุณ เข้าสู่ระบบ Office 365[ศูนย์การรักษาความปลอดภัยและการปฏิบัติตาม](https://protection.office.com/)นโยบาย
2. เลือก **การจัดการ** ภัยคุกคาม ในบานหน้าต่างด้านซ้าย จากนั้นเลือก นโยบาย **ตู้เซฟ**  >  [สิ่งที่แนบมา](https://protection.office.com/safeattachment)
3. **เลือก เปิด Microsoft Defender Office 365 SharePoint OneDrive Microsoft Teams** จากนั้นเลือก บันทึก
    > [!TIP]
    >
    > - ในฐานะผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบ SharePoint Online ให้เรียกใช้ cmdlet PowerShell ต่อไปนี้กับ **พารามิเตอร์ DisallowInfectedFileDownload** ที่ตั้งค่า *เป็น true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [ตั้งค่าการแจ้งเตือนไฟล์ที่ถูกตรวจพบ](https://go.microsoft.com/fwlink/?linkid=2092110)

ดูข้อมูลเพิ่มเติมใน Microsoft [Defender for Office 365 for SharePoint, OneDrive และ Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041)
