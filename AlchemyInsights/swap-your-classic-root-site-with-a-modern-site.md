---
title: สลับไซต์รากคลาสสิกของคุณด้วยไซต์ที่ทันสมัย
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691198"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>สลับไซต์รากคลาสสิกของคุณด้วยไซต์ที่ทันสมัย

ถ้าสภาพแวดล้อมของคุณถูกตั้งค่าก่อนเดือนเมษายน๒๐๑๙คุณสามารถเปลี่ยนไซต์รากของคุณไปยังไซต์ที่ทันสมัยได้โดยใช้ Microsoft PowerShell:

- ถ้าคุณมีไซต์ที่แตกต่างกันที่คุณต้องการใช้เป็นไซต์รากของคุณคุณสามารถแทนที่ [(swap) ไซต์ราก](https://docs.microsoft.com/sharepoint/modern-root-site) ด้วยได้ 
    - ใช้ [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) เพื่อสลับตำแหน่งที่ตั้งของไซต์กับไซต์อื่นในขณะที่เก็บถาวรไซต์ต้นฉบับ พร้อมใช้งานสำหรับไซต์ทีมทั้งสอง (ไม่ได้เชื่อมต่อกับกลุ่ม) และไซต์การติดต่อสื่อสาร 

- ความสามารถเพิ่มเติมจะได้รับการแนะนำในเร็วๆนี้ที่จะช่วยให้คุณสามารถใช้เนื้อหาบนไซต์ได้แต่แปลงไซต์ที่มีอยู่แล้วไปยังไซต์การติดต่อสื่อสาร 
>[!Important]
>ความสามารถเหล่านี้จะได้รับการรีดออกมาค่อยๆ ดำเนินการตรวจสอบศูนย์ข้อความสำหรับการอัปเดต 

## <a name="known-issues-with-swapping-sites"></a>ปัญหาที่ทราบเกี่ยวกับการสลับไซต์

- ไซต์เป้าหมายอาจส่งกลับข้อผิดพลาด "ไม่พบ" (HTTP ๔๐๔) เป็นระยะเวลาสั้นๆ
- เนื้อหาจะต้องถูก recrawled เพื่ออัปเดตดัชนีการค้นหา ไม่จำเป็นต้องมีขั้นตอนด้วยตนเอง-สิ่งนี้จะถูกดำเนินการโดยอัตโนมัติ
- สิ่งที่ขึ้นอยู่กับการเชื่อมโยง "คงที่" (เช่นไฟล์การซิงค์และไฟล์ OneNote) จะต้องได้รับการแก้ไขด้วยตนเอง
- ถ้าไซต์ต้นฉบับเป็นไซต์ข่าวสารขององค์กรให้อัปเดต URLรับรายการของไซต์ข่าวสารขององค์กรทั้งหมด
- ไซต์ Project Server อาจจำเป็นต้องมีการตรวจสอบความถูกต้องเพื่อให้แน่ใจว่าพวกเขายังคงเชื่อมโยงอย่างถูกต้อง
