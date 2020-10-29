---
title: เปิดใช้งาน Office ๓๖๕ ATP สำหรับ SharePoint, OneDrive และทีม Microsoft
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801094"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>เปิดใช้งาน Microsoft Defender สำหรับ Office ๓๖๕สำหรับ SharePoint Online, OneDrive และทีม Microsoft

1. ไปที่ https://protection.office.com แล้วลงชื่อเข้าใช้
2. เลือก **นโยบายการจัดการภัยคุกคาม**  >  **Policy**  >  **สิ่งที่แนบมาที่ปลอดภัย**
3. เลือก **เปิดใช้งาน ATP สำหรับ SharePoint, OneDrive และทีม Microsoft** แล้วคลิก **บันทึก**
4. แนะนำ ในฐานะผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบ SharePoint Online ให้เรียกใช้ cmdlet [SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)ที่มีการตั้งค่าพารามิเตอร์ **DisallowInfectedFileDownload** เป็น *true*
5. แนะนำ [ตั้งค่าการแจ้งเตือน](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) สำหรับไฟล์ที่ตรวจพบ

> [!NOTE]
> ATP จะ nto สแกนทุกไฟล์เดี่ยวใน SharePoint Online, OneDrive หรือทีม Microsoft ไฟล์จะสแกนแบบอะซิงโครนัสผ่านกระบวนการที่ใช้การแชร์และเหตุการณ์กิจกรรมของผู้เยี่ยมชมพร้อมกับสมาร์ทวริและสัญญาณการคุกคามเพื่อระบุไฟล์ที่เป็นอันตราย ให้ดูที่[ATP สำหรับ SharePoint, OneDrive และทีม Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)