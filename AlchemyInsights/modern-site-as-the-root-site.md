---
title: ไซต์สมัยใหม่เป็นไซต์ราก
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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000411"
---
# <a name="modern-site-as-root-site"></a>ไซต์สมัยใหม่เป็นไซต์ราก

We havegun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site). ใช้ [Invoke-SPOSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) เพื่อสลับที่ตั้งของไซต์กับไซต์อื่นในขณะที่เก็บถาวรไซต์เดิม พร้อมใช้งานทั้งไซต์ทีม (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การติดต่อสื่อสาร

>[!Important]
> อย่าลบไซต์รากแบบคลาสสิกของคุณเพื่อสร้างไซต์การติดต่อสื่อสารที่ทันสมัย Microsoft ไม่สนับสนุนเรื่องนี้ การลบไซต์รากจะSharePointไซต์หลักทั้งหมดในองค์กรของคุณไม่สามารถเข้าถึงผู้ใช้ทั้งหมดได้ จนกว่าคุณจะคืนค่าไซต์หรือสร้างไซต์ใหม่ที่ URL เดียวกัน เราจะติดต่อสื่อสารฟีเจอร์นี้ผ่านศูนย์ข้อความ คุณควรคาดว่าฟีเจอร์นี้จะเปิดใช้งานในผู้เช่าของคุณในไม่ช้า

## <a name="known-issues-with-swapping-sites"></a>ปัญหาที่ทราบเกี่ยวกับการสลับไซต์
- ไซต์เป้าหมายอาจส่งกลับข้อผิดพลาด "ไม่พบ" (HTTP 404) เป็นระยะเวลาสั้นๆ
- เนื้อหาจะต้องถูกลากเพื่ออัปเดตดัชนีการค้นหา ที่นี่ไม่ต้องมีขั้นตอนด้วยตนเอง ซึ่งจะเสร็จสิ้นโดยอัตโนมัติ
- สิ่งที่ขึ้นอยู่กับลิงก์ "แบบคงที่" (เช่น การซิงค์OneNoteไฟล์) จะต้องได้รับการแก้ไขด้วยตนเอง
- Project ไซต์เซิร์ฟเวอร์อาจต้องได้รับการตรวจสอบความถูกต้องเพื่อให้แน่ใจว่ายังคงเชื่อมโยงอย่างถูกต้อง 
