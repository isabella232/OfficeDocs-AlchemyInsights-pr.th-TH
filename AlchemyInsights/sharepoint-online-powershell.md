---
title: พาวเวอร์เชลล์ออนไลน์ของ SharePoint
ms.author: v-todmc
author: todmccoy
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
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764282"
---
# <a name="sharepoint-online-powershell"></a>พาวเวอร์เชลล์ออนไลน์ของ SharePoint

การทํางานกับ PowerShell หรือสคริปต์ภายใน Sharepoint แบบออนไลน์หรือไม่ ไปที่ลิงค์ด้านล่างสําหรับข้อมูลเพิ่มเติม
- [การเริ่มต้นใช้งานเชลล์การจัดการแบบออนไลน์ของ SharePoint](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [เชื่อมต่อกับ SPO PowerShell ด้วยการตรวจสอบสิทธิ์แบบหลายปัจจัย (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [รูปแบบและแนวปฏิบัติของ SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)ประกอบด้วยไลบรารีของคําสั่ง PowerShell ที่ช่วยให้คุณสามารถดําเนินการจัดการที่ซับซ้อนต่อ SPO

> [!NOTE]
> - ถ้าคุณกําลังมีปัญหาในการเชื่อมต่อกับเชลล์การจัดการ SPO โปรดตรวจสอบให้แน่ใจว่า คุณได้ปรับปรุงเป็นรุ่นล่าสุด และลอง[นําเข้าโมดูล](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module)โดยใช้ *"นําเข้าโมดูล Microsoft.SharePoint.SharePoint.PowerShell"* อีกครั้ง
> - ถ้าคุณกําลังพยายามเรียกใช้สคริปต์ของวัตถุฝั่งไคลเอ็นต์แบบจําลอง คุณจะต้องมี[SDK คอมโพเนนต์ของไคลเอ็นต์ออนไลน์ของ Sharepoint](https://www.microsoft.com/download/details.aspx?id=42038)ที่ติดตั้งบนเครื่องของคุณภายในเครื่อง
> - ถ้าคุณมีปัญหาการเรียกใช้สคริปต์จาก PowerShell คุณอาจต้องการพิจารณาการเรียกใช้ PowerShell เป็นผู้ดูแลระบบ และการเปลี่ยนแปลง[นโยบายการดําเนินการ](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)