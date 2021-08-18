---
title: ข้อจํากัดของป้ายชื่อระดับความลับOfficeไฟล์ในSharePointและOneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e2fc8fcf27eb916f64e4235cd116d9a7096e6078391e72363421ac3de721f5ee
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899783"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>ข้อจํากัดของป้ายชื่อระดับความลับOfficeไฟล์ในSharePointและOneDrive

เมื่อเปิดใช้งานป้ายชื่อระดับความลับOfficeไฟล์ใน SharePoint OneDriveโปรดระวังข้อจํากัดและข้อจํากัด ซึ่งรวมถึง:

- SharePoint และ OneDrive ไม่สามารถประมวลผลไฟล์บางไฟล์ที่มีป้ายชื่อและเข้ารหัสลับจากแอป Office บนเดสก์ท็อปได้เมื่อไฟล์มีข้อมูล PowerQuery ข้อมูลที่จัดเก็บโดย Add-in แบบเอง หรือส่วน XML แบบเอง
- SharePointและOneDriveความลับจะไม่ถูกใช้ป้ายชื่อระดับความลับกับไฟล์ที่มีอยู่ที่คุณได้เข้ารหัสลับไว้แล้วโดยใช้ป้ายชื่อ Azure Information Protection (AIP) โดยอัตโนมัติ เมื่อต้องการใช้ป้ายชื่อระดับความลับกับไฟล์ที่เข้ารหัสลับ: 
    - ตรวจสอบให้แน่ใจว่าป้ายชื่อ AIP ถูกโยกย้ายและเผยแพร่ไปยังศูนย์Microsoft 365การปฏิบัติตามข้อบังคับ
    - ดาวน์โหลดไฟล์ที่มีป้ายชื่อ แล้วอัปโหลดไปยังต้นฉบับSharePointหรือOneDriveที่ตั้งเดิม
- การพิมพ์ไม่ได้รับการสนับสนุนในเอกสารที่เข้ารหัสลับ

For additional details on limitations, see [Enable sensitivity labels for Office files in SharePoint and OneDrive](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations).
