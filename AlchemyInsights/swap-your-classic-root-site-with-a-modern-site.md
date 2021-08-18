---
title: สลับไซต์รากแบบคลาสสิกของคุณด้วยไซต์สมัยใหม่
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316159"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>สลับไซต์รากแบบคลาสสิกของคุณด้วยไซต์สมัยใหม่

ถ้าสภาพแวดล้อมของคุณถูกตั้งค่าก่อนเดือนเมษายน 2019 คุณสามารถเปลี่ยนไซต์รากของคุณไปยังไซต์สมัยใหม่โดยใช้ Microsoft PowerShell:

- If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it. 
    - ใช้ [Invoke-SPOSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) เพื่อสลับที่ตั้งของไซต์กับไซต์อื่นในขณะที่เก็บถาวรไซต์เดิม พร้อมใช้งานทั้งไซต์ทีม (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การติดต่อสื่อสาร 

- ความสามารถเพิ่มเติมจะเปิดตัวเร็วๆ นี้ ซึ่งจะอนุญาตให้คุณใช้เนื้อหาบนไซต์ต่อไปได้ แต่แปลงไซต์ที่มีอยู่เป็นไซต์การติดต่อสื่อสาร 

**สําคัญ**: ความสามารถเหล่านี้จะค่อยๆ ทยอยเปิดให้เล่น ตรวจสอบศูนย์ข้อความต่อไปเพื่ออัปเดต 

## <a name="known-issues-with-swapping-sites"></a>ปัญหาที่ทราบเกี่ยวกับการสลับไซต์

- ไซต์เป้าหมายอาจส่งกลับข้อผิดพลาด "ไม่พบ" (HTTP 404) เป็นระยะเวลาสั้นๆ
- เนื้อหาจะต้องถูกลากเพื่ออัปเดตดัชนีการค้นหา ไม่ต้องมีขั้นตอนด้วยตนเอง ซึ่งจะเสร็จสิ้นโดยอัตโนมัติ
- สิ่งที่ขึ้นอยู่กับลิงก์ "แบบคงที่" (เช่น ซิงค์OneNoteไฟล์) จะต้องได้รับการแก้ไขด้วยตนเอง
- ถ้าไซต์ต้นทางเป็นไซต์ข่าวสารขององค์กร ให้อัปเดต URL รับรายการไซต์ข่าวสารขององค์กรทั้งหมด
- Project ไซต์เซิร์ฟเวอร์อาจต้องได้รับการตรวจสอบความถูกต้องเพื่อให้แน่ใจว่ายังคงเชื่อมโยงอย่างถูกต้อง
