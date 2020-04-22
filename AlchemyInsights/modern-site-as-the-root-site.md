---
title: เว็บไซต์ที่ทันสมัยเป็นไซต์ราก
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713810"
---
# <a name="modern-site-as-root-site"></a>ไซต์ที่ทันสมัยเป็นไซต์ราก

เราได้เริ่มที่จะเปิดตัวคุณลักษณะใหม่ที่จะช่วยให้คุณ[แลกเปลี่ยนเว็บไซต์รากเว็บไซต์คลาสสิกของคุณกับเว็บไซต์ที่ทันสมัย](https://docs.microsoft.com/sharepoint/modern-root-site) ใช้[Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)เพื่อสลับตําแหน่งของไซต์กับไซต์อื่นในขณะที่เก็บไซต์เดิม พร้อมใช้งานสําหรับไซต์ทีม (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การติดต่อสื่อสาร

>[!Important]
> อย่าลบไซต์รากของคุณคลาสสิกเพื่อสร้างไซต์การสื่อสารที่ทันสมัย ซึ่งไม่ได้รับการสนับสนุนโดย Microsoft การลบไซต์รากจะทําให้ไซต์ SharePoint ทั้งหมดในองค์กรของคุณไม่สามารถเข้าถึงได้กับผู้ใช้ทุกคน จนกว่าคุณจะคืนค่าไซต์หรือสร้างไซต์ใหม่ที่ URL เดียวกัน เราจะสื่อสารคุณลักษณะนี้ผ่านทางศูนย์ข้อความ คุณควรคาดหวังว่าคุณลักษณะที่จะเปิดใช้งานในผู้เช่าของคุณในไม่ช้า

## <a name="known-issues-with-swapping-sites"></a>ปัญหาที่ทราบเกี่ยวกับการแลกเปลี่ยนไซต์
- ไซต์เป้าหมายอาจส่งคืนข้อผิดพลาด "ไม่พบ" (HTTP 404) เป็นระยะเวลาสั้น ๆ
- เนื้อหาจะต้องถูกตระเวนใหม่เพื่อปรับปรุงดัชนีการค้นหา ไม่มีขั้นตอนด้วยตนเองที่จําเป็นที่นี่, นี้จะกระทําโดยอัตโนมัติ.
- สิ่งที่ขึ้นอยู่กับการเชื่อมโยง "แบบคงที่" (เช่น File Sync และไฟล์ OneNote) จะต้องถูกแก้ไขด้วยตนเอง
- ไซต์เซิร์ฟเวอร์โครงการอาจต้องถูกตรวจสอบเพื่อให้แน่ใจว่า พวกเขายังคงเชื่อมโยงอย่างถูกต้อง 
