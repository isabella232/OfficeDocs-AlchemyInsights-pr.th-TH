---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830601"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

ต้องใช้งาน PowerShell หรือสคริปต์ภายใน Sharepoint Online ใช่ไหม ไปที่ลิงก์ด้านล่างเพื่อดูข้อมูลเพิ่มเติม
- [เริ่มต้นใช้งาน SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [เชื่อมต่อกับ SPO PowerShell ที่มีการรับรองความถูกต้องแบบหลายปัจจัย (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [รูปแบบและหลักปฏิบัติของ SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) มีไลบรารีของสั่ง PowerShell ที่ช่วยให้คุณจัดการการจัดการที่ซับซ้อนต่อ SPO ได้

> [!NOTE]
> - ถ้าคุณพบปัญหาในการเชื่อมต่อกับเชลล์การจัดการ SPO ให้ตรวจสอบให้แน่ใจว่าคุณได้อัปเดตเป็นเวอร์ชันล่าสุดแล้ว และลองนําเข้าโมดูลอีกครั้งโดยใช้ *"นําเข้า-มอดูล Microsoft.Online.SharePoint.PowerShell"* [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1)
> - ถ้าคุณพยายามเรียกใช้สคริปต์โมเดลวัตถุฝั่งไคลเอ็นต์ คุณจะต้องติดตั้ง [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) บนเครื่องของคุณ
> - If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).