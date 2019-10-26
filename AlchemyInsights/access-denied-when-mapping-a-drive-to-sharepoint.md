---
title: การเข้าถึงถูกปฏิเสธเมื่อทำการแมปไดรฟ์ไปยัง SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/25/2019
ms.locfileid: "36737496"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a>แก้ไขปัญหาเกี่ยวกับไลบรารี SharePoint ที่ถูกแมปไปยังไดรฟ์เครือข่าย

เมื่อคุณเรียกดูไปยังไดรฟ์เครือข่ายที่แมปคุณอาจเห็นหนึ่งในข้อความต่อไปนี้:
  
- **\\เส้นทางไม่สามารถเข้าถึงได้ คุณอาจไม่มีสิทธิ์ในการใช้ทรัพยากรเครือข่ายนี้ ติดต่อผู้ดูแลของเซิร์ฟเวอร์นี้เพื่อดูว่าคุณมีสิทธิ์การเข้าถึงหรือไม่**

- **ปฏิเสธการเข้าถึง ก่อนที่จะเปิดแฟ้มในตำแหน่งนี้คุณต้องเพิ่มเว็บไซต์ลงในรายการไซต์ที่เชื่อถือได้ของคุณก่อนเรียกดูเว็บไซต์และเลือกตัวเลือกเพื่อเข้าสู่ระบบโดยอัตโนมัติ**

[รับความช่วยเหลือในการแก้ปัญหาไดรฟ์เครือข่ายที่แมป](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)ไว้
  
การแมปไลบรารีเป็นไดรฟ์เครือข่ายเป็นแบบถาวรและได้รับการสนับสนุนใน Internet Explorer เท่านั้น ให้[ซิงค์แฟ้ม SharePoint กับไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)ซึ่งมี[แฟ้มตามความต้อง](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)การแทน เข้าถึงไฟล์ทั้งหมดของคุณใน OneDrive โดยไม่ต้องใช้พื้นที่จัดเก็บข้อมูลภายใน
  