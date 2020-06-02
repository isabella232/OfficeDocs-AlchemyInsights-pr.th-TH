---
title: เปิดใช้งาน ATP ของ Office 365 สําหรับ SharePoint, OneDrive และทีม Microsoft
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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506937"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>เปิดใช้งานการป้องกันภัยคุกคามขั้นสูงของ Office 365 สําหรับ SharePoint แบบออนไลน์, OneDrive และทีม Microsoft

1. ไปที่ https://protection.office.com และลงชื่อเข้าใช้
2. เลือก**นโยบายการจัดการภัยคุกคาม**  >  **Policy**  >  **สิ่งที่แนบมาที่ปลอดภัย**
3. เลือก**เปิด ATP สําหรับ SharePoint, OneDrive และ ทีม Microsoft**แล้วคลิก**บันทึก**
4. (แนะนํา) ในฐานะผู้ดูแลส่วนกลางหรือผู้ดูแล SharePoint Online เรียกใช้ cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)ด้วยการตั้งค่าพารามิเตอร์**DisallowInfectedFileDownload**เป็น*true*
5. (แนะนํา) [ตั้งค่าการแจ้งเตือน](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)สําหรับแฟ้มที่ตรวจพบ

> [!NOTE]
> ATP จะสแกนทุกแฟ้มเดียวใน SharePoint แบบออนไลน์, OneDrive หรือ Microsoft Teams ไฟล์จะถูกสแกนแบบอะซิงโครนัสผ่านกระบวนการที่ใช้กิจกรรมร่วมกันและกิจกรรมของแขกพร้อมกับ heuristics สมาร์ทและสัญญาณภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย ดู[ATP สําหรับ SharePoint, OneDrive และทีม Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)