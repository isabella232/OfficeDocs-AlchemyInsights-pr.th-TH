---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709089"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

ต้องการใช้งาน PowerShell หรือสคริปต์ภายใน Sharepoint Online ใช่ไหม ไปที่ลิงก์ด้านล่างเพื่อดูข้อมูลเพิ่มเติม
- [เริ่มต้นใช้งาน SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [เชื่อมต่อกับ SPO PowerShell ที่มีการรับรองความถูกต้องแบบหลายปัจจัย (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [รูปแบบและหลักปฏิบัติของ SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) มีไลบรารีของสั่ง PowerShell ที่ช่วยให้คุณสามารถจัดการที่ซับซ้อนต่อ SPO ได้

> [!NOTE]
> - ถ้าคุณมีปัญหาในการเชื่อมต่อกับเชลล์การจัดการ SPO ตรวจสอบให้แน่ใจว่าคุณได้อัปเดตเป็นเวอร์ชันล่าสุดแล้วและพยายามนําเข้ามอดูลอีกครั้งโดยใช้ *"Import-Module Microsoft.Online.SharePoint.PowerShell"* [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1)
> - ถ้าคุณพยายามเรียกใช้สคริปต์โมเดลวัตถุที่ฝั่งไคลเอ็นต์ คุณจะต้องติดตั้ง [SharePoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) บนเครื่องของคุณ
> - If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).