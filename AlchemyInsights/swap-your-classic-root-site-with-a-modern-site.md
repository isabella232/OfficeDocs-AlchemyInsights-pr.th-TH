---
title: สลับเว็บไซต์รากคลาสสิกของคุณกับเว็บไซต์ที่ทันสมัย
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741563"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>สลับเว็บไซต์รากคลาสสิกของคุณกับเว็บไซต์ที่ทันสมัย

ถ้าสภาพแวดล้อมของคุณถูกตั้งค่าก่อนเดือนเมษายน 2019 คุณสามารถเปลี่ยนไซต์รากของคุณเป็นไซต์ที่ทันสมัย โดยใช้ Microsoft PowerShell:

- หากคุณมีเว็บไซต์อื่นที่คุณต้องการใช้เป็นไซต์รากของคุณคุณสามารถแทนที่[(swap) ไซต์ราก](https://docs.microsoft.com/sharepoint/modern-root-site)กับมัน 
    - ใช้[Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)เพื่อสลับตําแหน่งของไซต์กับไซต์อื่นในขณะที่เก็บไซต์เดิม พร้อมใช้งานสําหรับไซต์ทีม (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การติดต่อสื่อสาร 

- ความสามารถเพิ่มเติมจะถูกนํามาใช้ในเร็ว ๆ นี้ที่จะช่วยให้คุณเพื่อให้การใช้เนื้อหาในเว็บไซต์ แต่แปลงเว็บไซต์ที่มีอยู่ไปยังไซต์การสื่อสาร 
>[!Important]
>ความสามารถเหล่านี้จะถูกรีดออกค่อยๆ ตรวจสอบการปรับปรุงศูนย์ข้อความต่อไป 

## <a name="known-issues-with-swapping-sites"></a>ปัญหาที่ทราบเกี่ยวกับการแลกเปลี่ยนไซต์

- ไซต์เป้าหมายอาจส่งคืนข้อผิดพลาด "ไม่พบ" (HTTP 404) เป็นระยะเวลาสั้น ๆ
- เนื้อหาจะต้องถูกตระเวนใหม่เพื่อปรับปรุงดัชนีการค้นหา ไม่มีขั้นตอนด้วยตนเองที่จําเป็น - นี้จะทําโดยอัตโนมัติ
- สิ่งที่ขึ้นอยู่กับการเชื่อมโยง "แบบคงที่" (เช่น File Sync และไฟล์ OneNote) จะต้องถูกแก้ไขด้วยตนเอง
- ถ้าไซต์ต้นทางเป็นไซต์ข่าวสารขององค์กร ให้อัปเดต URLดูรายการไซต์ข่าวสารขององค์กรทั้งหมด
- ไซต์เซิร์ฟเวอร์โครงการอาจต้องถูกตรวจสอบเพื่อให้แน่ใจว่า พวกเขายังคงเชื่อมโยงอย่างถูกต้อง
