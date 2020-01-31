---
title: ไม่สามารถลบรายการใน SharePoint หรือ OneDrive ได้
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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571290"
---
# <a name="unable-to-delete-items"></a>ไม่สามารถลบรายการ

นโยบายการเก็บข้อมูลอาจทำให้เกิดปัญหานี้คุณจำเป็นต้องปิดใช้งานหรือไม่รวมการระงับที่เกี่ยวข้องกับสาเหตุนี้ หลังจากที่นโยบายการเก็บข้อมูลหรือระงับไว้จะถูกเอาออกอาจใช้เวลาถึง24ชั่วโมงสำหรับการเปลี่ยนแปลงจะมีผล ตรวจสอบให้แน่ใจว่าไม่มีการตั้งค่า[นโยบายการเก็บข้อมูล](https://docs.microsoft.com/office365/securitycompliance/retention-policies)บนสินค้า

ไซต์อาจเกินขีดจำกัดการเก็บข้อมูลเพิ่ม[โควตาของไซต์](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)และลบรายการ

ตรวจสอบให้แน่ใจว่าสินค้าไม่ได้ถูก[เช็คเอาท์](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)ไปยังผู้ใช้อื่น

ในที่สุดผู้ดูแลระบบสามารถใช้[รูปแบบของ SharePoint และวิธีปฏิบัติ](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP) ซึ่งประกอบด้วยไลบรารีของคำสั่ง PowerShell ที่ช่วยให้คุณสามารถทำการดำเนินการจัดการที่ซับซ้อนเช่นบังคับการลบรายการที่เป็นปาก
- [เอาแฟ้ม PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [เอาโฟลเดอร์ PNP ออก](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [เอารายการ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [เอารายการ PNP](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [เอาเขตข้อมูล PNP (คอลัมน์)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)