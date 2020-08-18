---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786908"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

การทำงานกับ PowerShell หรือสคริปต์ภายใน Sharepoint Online หรือไม่ ไปที่ลิงก์ทางด้านล่างเพื่อดูข้อมูลเพิ่มเติม
- [การเริ่มต้นใช้งาน SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [เชื่อมต่อกับ SPO PowerShell ที่มีการรับรองความถูกต้องรับรอง (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [รูปแบบและหลักปฏิบัติของ SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) มีไลบรารีของคำสั่ง PowerShell ที่ช่วยให้คุณสามารถดำเนินการการจัดการที่ซับซ้อนต่อ SPO

> [!NOTE]
> - ถ้าคุณกำลังมีปัญหาในการเชื่อมต่อกับ SPO management shell ตรวจสอบให้แน่ใจว่าคุณได้อัปเดตเป็นเวอร์ชันล่าสุดแล้วลอง [นำเข้าโมดูลใหม่](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) โดยใช้ *"นำเข้าโมดูลของไมโครซอฟท์ออนไลน์. PowerShell"*
> - ถ้าคุณกำลังพยายามเรียกใช้สคริปต์รูปแบบวัตถุฝั่งไคลเอ็นต์คุณจำเป็นต้องมีการติดตั้ง [SDK คอมโพเนนต์ของไคลเอ็นต์ Sharepoint Online](https://www.microsoft.com/download/details.aspx?id=42038) ไว้บนเครื่องภายในเครื่องของคุณ
> - ถ้าคุณกำลังมีปัญหาในการเรียกใช้สคริปต์จาก PowerShell คุณอาจต้องการพิจารณาเรียกใช้ PowerShell ในฐานะผู้ดูแลระบบและการเปลี่ยนแปลง [นโยบายการดำเนิน](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)การ