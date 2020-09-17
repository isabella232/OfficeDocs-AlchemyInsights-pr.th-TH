---
title: ไม่สามารถลบรายการใน SharePoint หรือ OneDrive ได้
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806130"
---
# <a name="unable-to-delete-items"></a>ไม่สามารถลบรายการได้

นโยบายการเก็บข้อมูลอาจทำให้เกิดปัญหานี้ได้คุณจำเป็นต้องปิดใช้งานหรือไม่รวมการระงับที่เป็นสาเหตุของปัญหานี้ หลังจากที่นโยบายการเก็บข้อมูลหรือการระงับถูกเอาออกอาจใช้เวลาถึง24ชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล ตรวจสอบให้แน่ใจว่าไม่มีการตั้งค่า [นโยบายการเก็บข้อมูล](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) ในรายการ

ไซต์อาจเกินขีดจำกัดที่เก็บข้อมูลเพิ่ม [โควตาของไซต์](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) และลบรายการ

ตรวจสอบให้แน่ใจว่ารายการไม่ได้ถูก [เช็คเอาท์](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) ไปยังผู้ใช้อื่น

ในที่สุดผู้ดูแลระบบสามารถใช้ [รูปแบบของ SharePoint และวิธีปฏิบัติ](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ซึ่งมีไลบรารีของคำสั่ง PowerShell ที่ช่วยให้คุณสามารถดำเนินการการจัดการที่ซับซ้อนเช่นบังคับให้มีการลบรายการที่เป็นปาก
- [เอาไฟล์ PNP ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [เอาโฟลเดอร์ PNP ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [เอารายการ PNP ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [เอารายการ PNP ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [เอาเขตข้อมูล PNP (คอลัมน์) ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)