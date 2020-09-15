---
title: ไซต์ที่ทันสมัยเป็นไซต์ราก
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666889"
---
# <a name="modern-site-as-root-site"></a>ไซต์ที่ทันสมัยเป็นไซต์ราก

เราได้เริ่มต้นใช้งานฟีเจอร์ใหม่ที่จะช่วยให้คุณสามารถ [สลับไซต์รากของไซต์แบบคลาสสิกของคุณกับไซต์ที่ทันสมัย](https://docs.microsoft.com/sharepoint/modern-root-site)ได้ไวร์ ใช้ [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) เพื่อสลับตำแหน่งที่ตั้งของไซต์กับไซต์อื่นในขณะที่เก็บถาวรไซต์ต้นฉบับ พร้อมใช้งานสำหรับไซต์ทีมทั้งสอง (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การติดต่อสื่อสาร

>[!Important]
> อย่าลบไซต์รากคลาสสิกของคุณเพื่อสร้างไซต์การติดต่อสื่อสารที่ทันสมัย การทำเช่นนี้ไม่ได้รับการสนับสนุนโดยไมโครซอฟท์ การลบไซต์รากจะทำให้ไซต์ SharePoint ทั้งหมดในองค์กรของคุณไม่สามารถเข้าถึงผู้ใช้ทั้งหมดได้จนกว่าคุณจะคืนค่าไซต์หรือสร้างไซต์ใหม่ที่ URL เดียวกัน เราจะทำการสื่อสารฟีเจอร์นี้ผ่านทางศูนย์ข้อความ คุณควรคาดหวังว่าฟีเจอร์นี้จะเปิดใช้งานในผู้เช่าของคุณในไม่ช้า

## <a name="known-issues-with-swapping-sites"></a>ปัญหาที่ทราบเกี่ยวกับการสลับไซต์
- ไซต์เป้าหมายอาจส่งกลับข้อผิดพลาด "ไม่พบ" (HTTP ๔๐๔) เป็นระยะเวลาสั้นๆ
- เนื้อหาจะต้องถูก recrawled เพื่ออัปเดตดัชนีการค้นหา ไม่จำเป็นต้องมีขั้นตอนด้วยตนเองที่นี่การดำเนินการนี้จะดำเนินการโดยอัตโนมัติ
- สิ่งที่ขึ้นอยู่กับการเชื่อมโยง "คงที่" (เช่นไฟล์การซิงค์และไฟล์ OneNote) จะต้องได้รับการแก้ไขด้วยตนเอง
- ไซต์ Project Server อาจจำเป็นต้องมีการตรวจสอบความถูกต้องเพื่อให้แน่ใจว่าพวกเขายังคงเชื่อมโยงอย่างถูกต้อง 
