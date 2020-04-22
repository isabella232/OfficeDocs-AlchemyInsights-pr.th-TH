---
title: เปิดใช้งาน ATP 365 ของ Office สําหรับ SharePoint, OneDrive และทีม Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703445"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>เปิดใช้งานการป้องกันภัยคุกคามขั้นสูงของ Office 365 สําหรับ SharePoint แบบออนไลน์ OneDrive และทีมของ Microsoft

1. ไปที่https://protection.office.comและลงชื่อเข้าใช้
2. เลือก**สิ่งที่แนบมาที่ปลอดภัย****ของนโยบาย** > **การจัดการภัยคุกคาม** > 
3. เลือก**เปิด ATP สําหรับ SharePoint, OneDrive และ ทีม Microsoft**แล้วคลิก**บันทึก**
4. (แนะนํา) ในฐานะผู้ดูแลระบบส่วนกลางหรือผู้ดูแล SharePoint แบบออนไลน์ เรียกใช้ cmdlet[ชุด SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)ด้วยพารามิเตอร์**DisallowInFectedFileDownload**ตั้งค่า*เป็น true*
5. (แนะนํา) [ตั้งค่าการแจ้งเตือน](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)สําหรับไฟล์ที่ตรวจพบ

> [!NOTE]
> ATP จะ nto สแกนทุกแฟ้มเดียวใน SharePoint แบบออนไลน์, OneDrive หรือทีม Microsoft ไฟล์จะถูกสแกนแบบอะซิงโครนัสผ่านกระบวนการที่ใช้กิจกรรมร่วมกันและกิจกรรมของแขกพร้อมกับการวิเคราะห์พฤติกรรมอัจฉริยะและสัญญาณภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย ดู[https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)