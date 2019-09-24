---
title: PowerShell แบบออนไลน์ของ Sharepoint
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123017"
---
# <a name="sharepoint-online-powershell"></a>PowerShell แบบออนไลน์ของ Sharepoint

การทำงานกับ PowerShell หรือสคริปต์ภายใน Sharepoint แบบออนไลน์หรือไม่ โปรดไปที่ลิงก์ด้านล่างเพื่อดูข้อมูลเพิ่มเติม
- [การเริ่มต้นใช้งานเชลล์จัดการออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [เชื่อมต่อกับการตรวจสอบหลายปัจจัย (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [รูปแบบและวิธีปฏิบัติของ SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)ประกอบด้วยไลบรารีของคำสั่ง PowerShell ที่ช่วยให้คุณสามารถดำเนินการจัดการที่ซับซ้อนไปยังที่ได้

> [!NOTE]
> - ถ้าคุณกำลังมีปัญหาในการเชื่อมต่อกับเชลล์จัดการใหม่ตรวจสอบให้แน่ใจว่าคุณได้ปรับปรุงเป็นรุ่นล่าสุดและพยายามที่จะ[นำเข้าโมดูล](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module)โดยใช้ *"นำเข้าโมดูล Microsoft. PowerShell"*
> - ถ้าคุณกำลังพยายามเรียกใช้สคริปต์รูปแบบวัตถุฝั่งไคลเอ็นต์คุณจะต้องมี[SDK คอมโพเนนต์ของไคลเอ็นต์ Sharepoint แบบออนไลน์](https://www.microsoft.com/download/details.aspx?id=42038)ที่ติดตั้งบนเครื่องของคุณ
> - ถ้าคุณกำลังมีปัญหาในการเรียกใช้สคริปต์จาก PowerShell คุณอาจต้องการพิจารณาเรียกใช้ PowerShell ในฐานะผู้ดูแลและการเปลี่ยนแปลง[นโยบายการดำเนิน](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)การ