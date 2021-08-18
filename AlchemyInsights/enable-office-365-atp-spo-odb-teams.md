---
title: เปิดใช้งานOffice 365 ATP SharePoint OneDrive และMicrosoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332178"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>เปิดใช้งาน Microsoft Defender Office 365 for SharePoint Online, OneDrive และ Microsoft Teams

1. ไปที่ https://protection.office.com และลงชื่อเข้าใช้
2. เลือก **นโยบาย**  >  **การจัดการ**  >  **ตู้เซฟ สิ่งที่แนบมา**
3. **เลือก เปิด Defender Office 365 SharePoint OneDrive Microsoft Teams** Defender **แล้วคลิก** บันทึก
4. (แนะนนะให้) ในฐานะผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบ SharePoint Online ให้เรียกใช้ cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)ด้วย **พารามิเตอร์ DisallowInfectedFileDownload** ที่ *ตั้งค่าเป็น true*
5. (แนะนนะให้) [ตั้งค่าการแจ้งเตือน](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) ไฟล์ที่ถูกตรวจพบ

**หมายเหตุ**: Microsoft Defender Office 365จะไม่สแกนทุกไฟล์ใน SharePoint Online, OneDrive หรือ Microsoft Teams ไฟล์จะถูกสแกนแบบอะซิงโครนัสผ่านกระบวนการที่ใช้เหตุการณ์กิจกรรมการแชร์และเหตุการณ์กิจกรรมของแขก พร้อมกับพฤติกรรมที่ชาญฉลาดและภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย ดู[Microsoft Defender Office 365 SharePoint OneDrive Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
