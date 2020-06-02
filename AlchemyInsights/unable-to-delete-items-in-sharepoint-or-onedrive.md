---
title: ไม่สามารถลบรายการใน SharePoint หรือ OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511995"
---
# <a name="unable-to-delete-items"></a>ไม่สามารถลบรายการ

นโยบายการเก็บข้อมูลอาจทําให้เกิดปัญหานี้ คุณจําเป็นต้องปิดใช้งานหรือยกเว้นการหยุดที่เกี่ยวข้องที่เป็นสาเหตุของปัญหานี้ หลังจากลบนโยบายการเก็บข้อมูลหรือการเก็บรักษาแล้ว อาจใช้เวลาถึง 24 ชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล ตรวจสอบให้แน่ใจว่าไม่มีการตั้งค่า[นโยบายการเก็บข้อมูล](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)บนรายการ

ไซต์อาจเกินขีดจํากัดของพื้นที่เก็บข้อมูล ให้เพิ่ม[โควต้าไซต์](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)และลบรายการนั้น

ตรวจสอบให้แน่ใจว่ารายการไม่ได้ถูก[เช็คเอาท์](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)ไปยังผู้ใช้อื่น

สุดท้าย ผู้ดูแลระบบสามารถใช้[รูปแบบและวิธีปฏิบัติของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) ซึ่งประกอบด้วยไลบรารีของคําสั่ง PowerShell ที่อนุญาตให้คุณดําเนินการจัดการที่ซับซ้อนเช่นบังคับให้ลบรายการปากแข็ง
- [เอาแฟ้ม PNP ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [ลบโฟลเดอร์ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [เอารายการ PNP ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [ลบรายการ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [เอาเขตข้อมูล PNP ออก (คอลัมน์)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)