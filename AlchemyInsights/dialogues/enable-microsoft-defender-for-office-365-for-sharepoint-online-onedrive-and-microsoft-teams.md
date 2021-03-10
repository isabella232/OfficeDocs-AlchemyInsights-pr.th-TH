---
title: เปิดใช้งาน Microsoft Defender for Office 365 for SharePoint Online, OneDrive และ Microsoft Teams
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
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695656"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>เปิดใช้งาน Microsoft Defender for Office 365 for SharePoint Online, OneDrive และ Microsoft Teams

1. ใช้ข้อมูลรับรองความถูกต้องของผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบความปลอดภัยของคุณ เข้าสู่ระบบศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายของ[Office 365](https://protection.office.com/)
2. เลือก **การจัดการ** ภัยคุกคามในบานหน้าต่างด้านซ้าย จากนั้นเลือก  >  [นโยบายสิ่งที่แนบมา](https://protection.office.com/safeattachment)ที่ปลอดภัย
3. เลือก **เปิด Microsoft Defender for Office 365 for SharePoint, OneDrive** และ Microsoft Teams **จากนั้นเลือก** บันทึก
    > [!TIP]
    >
    > - ในฐานะผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบ SharePoint Online ให้เรียกใช้ cmdlet PowerShell ต่อไปนี้ด้วยพารามิเตอร์ **DisallowInfectedFileDownload** ถูกตั้งค่า *เป็น true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [ตั้งค่าการแจ้งเตือนไฟล์ที่ถูกตรวจพบ](https://go.microsoft.com/fwlink/?linkid=2092110)

For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
