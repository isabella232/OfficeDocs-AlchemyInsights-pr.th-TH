---
title: เปิดใช้งาน Office 365 ATP สำหรับ SharePoint, OneDrive และทีม งานของ Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031118"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>เปิดใช้งานการป้องกันการคุกคามขั้นสูง 365 Office สำหรับ SharePoint แบบออนไลน์ OneDrive และทีม งานของ Microsoft

1. ไปที่https://protection.office.comและเข้าสู่ระบบ
2. เลือก**จัดการความเสี่ยง** > **นโยบาย** > **สิ่งที่แนบมาที่ปลอดภัย**
3. เลือก**เปิด ATP สำหรับ SharePoint, OneDrive และทีมงาน Microsoft**และจากนั้น คลิก**บันทึก**
4. (แนะนำ) เป็นผู้ดูแลส่วนกลางหรือผู้ดูแล SharePoint แบบออนไลน์ เรียกใช้ cmdlet[ชุด SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)ที่ มีพารามิเตอร์**DisallowInfectedFileDownload**ตั้งค่าเป็น*true*
5. (แนะนำ) [ตั้งค่าการแจ้งเตือน](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)สำหรับแฟ้มที่ตรวจพบ

> [!NOTE]
> ATP จะสแกน n หากทุกแฟ้มเดียวใน SharePoint แบบออนไลน์ OneDrive หรือทีม งานของ Microsoft แฟ้มที่จะสแกนแบบอะซิงโครนัส ตลอดกระบวนการที่ใช้ร่วมกัน และบัญชี guest กิจกรรมเหตุการณ์ การศึกษาสำนึกสมาร์ทและการคุกคามสัญญาณเพื่อระบุแฟ้มที่เป็นอันตราย ดู[https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)