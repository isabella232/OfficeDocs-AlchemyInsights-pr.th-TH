---
title: ไม่สามารถลบรายการในSharePointหรือOneDrive
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
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038536"
---
# <a name="unable-to-delete-items"></a>ไม่สามารถลบรายการได้

- นโยบายการเก็บข้อมูลอาจทําให้เกิดปัญหานี้ คุณจึงต้องปิดใช้งานหรือแยกการหยุดที่เกี่ยวข้องที่เป็นสาเหตุของปัญหานี้ หลังจากนโยบายการเก็บข้อมูลหรือหยุดถูกเอาออก อาจใช้เวลาถึง 24 ชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล ตรวจสอบให้แน่ใจว่าไม่มี [การตั้งค่านโยบายการเก็บ](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) ข้อมูลบนรายการ

- ไซต์อาจมีที่เก็บข้อมูลเกินขีดจํากัด เพิ่ม [โควตา](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ของไซต์และลบรายการนั้น

- ตรวจสอบให้แน่ใจว่าไม่ได้ [เช็คเอาท์รายการ](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) กับผู้ใช้อื่น

- สุดท้าย ผู้ดูแลระบบสามารถใช้รูปแบบและหลัก[ปฏิบัติของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ซึ่งมีไลบรารีของสั่ง PowerShell ที่อนุญาตให้คุณจัดการที่ซับซ้อน เช่น บังคับลบรายการสเตนซอร์ส
- [ลบไฟล์ PNP ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [เอาโฟลเดอร์ PNP ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [เอาข้อมูลในรายการ PNP ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [ลบรายการ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [เอาเขตข้อมูล PNP (คอลัมน์) ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)