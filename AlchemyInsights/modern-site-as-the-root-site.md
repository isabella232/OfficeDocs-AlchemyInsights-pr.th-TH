---
title: สมัยใหม่ไซต์เป็นไซต์ราก
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057787"
---
# <a name="modern-site-as-root-site"></a>สมัยใหม่ไซต์เป็นไซต์ราก

ลูกค้า[เป้าหมายย่อย](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide)ในขณะนี้สามารถเปิดใช้งานประสบการณ์การใช้งานไซต์ของการสื่อสารแบบสมัยใหม่ที่ไซต์รากคลาสสิกของผู้เช่าของ SharePoint

คุณลักษณะนี้สามารถเรียกใช้ โดยการเรียกใช้ cmdlet PowerShell แบบง่าย ๆ ในการดำเนินการเสร็จสมบูรณ์ของ PowerShell command(s) ไซต์รากจะมีการสื่อสารไซต์โฮมเพจใหม่ รายละเอียดเกี่ยวกับ PowerShell cmdlet และคุณลักษณะความต้องการไม่มีอยู่ในบทความ[SPOCommSite เปิดใช้งาน](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps) 

เราจะสามารถค่อย ๆ ย้อนนี้ออก ปิด โดยค่าเริ่มต้น ไปยังลูกค้าเป้าหมายย่อยใน 2019 พฤษภาคมล่วงหน้า และแบบโรออกจะใช้บริการทั่วโลก โดยจุดสิ้นสุดของเดือน 2019 มิถุนายน ดำเนินต่อเพื่ออ้างอิงไปยัง[ศูนย์ข้อความ](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)สำหรับคุณลักษณะใหม่อื่น ๆ ด้วยแบบสมัยใหม่ 

**สิ่งสำคัญ**: อย่าลบไซต์รากคลาสสิกของการสร้างไซต์สื่อสารแบบสมัยใหม่ นี้จะไม่ได้รับการสนับสนุน โดย Microsoft การลบไซต์รากจะทำให้ไซต์ SharePoint ทั้งหมดในองค์กรของคุณไม่สามารถเข้าถึงผู้ใช้ทั้งหมด จนกว่าคุณคืนค่าไซต์ หรือสร้างไซต์ใหม่ที่ URL เดียวกัน 
 
 