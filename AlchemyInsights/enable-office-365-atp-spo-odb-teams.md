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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543947"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>เปิดใช้งาน Microsoft Defender Office 365 for SharePoint Online, OneDrive และ Microsoft Teams

1. ไปที่ https://protection.office.com และลงชื่อเข้าใช้
2. เลือก **นโยบาย**  >  **การจัดการ**  >  **ภัยคุกคาม สิ่งที่แนบมา** ที่ปลอดภัย
3. **เลือก เปิด Defender Office 365 SharePoint OneDrive Microsoft Teams** Defender **แล้วคลิก** บันทึก
4. (แนะนนะให้) ในฐานะผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบ SharePoint Online ให้เรียกใช้ cmdlet [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)ด้วย **พารามิเตอร์ DisallowInfectedFileDownload** ที่ *ตั้งค่าเป็น true*
5. (แนะนนะให้) [ตั้งค่าการแจ้งเตือน](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) ไฟล์ที่ถูกตรวจพบ

> [!NOTE]
> Microsoft Defender Office 365จะไม่สแกนทุกไฟล์ใน SharePoint Online, OneDrive หรือ Microsoft Teams ไฟล์จะถูกสแกนแบบอะซิงโครนัสผ่านกระบวนการที่ใช้เหตุการณ์กิจกรรมการแชร์และเหตุการณ์กิจกรรมของแขก พร้อมกับพฤติกรรมที่ชาญฉลาดและภัยคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย ดู[Microsoft Defender Office 365 SharePoint OneDrive Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)