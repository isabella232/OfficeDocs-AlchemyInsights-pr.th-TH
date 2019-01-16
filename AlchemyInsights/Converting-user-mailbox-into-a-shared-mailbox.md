---
title: แปลงกล่องจดหมายของผู้ใช้ลงในกล่องจดหมายที่ใช้ร่วมกันได้อย่างไร
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28317053"
---
<span data-ttu-id="0d3fa-p101">คุณสามารถแปลงได้เฉพาะกล่องจดหมายของผู้ใช้ไปยังกล่องจดหมายที่ใช้ร่วมกันถ้าผู้ใช้มีสิทธิ์การใช้งานของการแลกเปลี่ยน หลังจากกล่องจดหมายจะถูกแปลง จะยังคงแสดงอยู่ในรายการผู้ใช้ที่ใช้งานอยู่ได้เนื่องจากรายการที่มีกล่องจดหมายที่ใช้ร่วมกัน อย่างไรก็ตาม กล่องจดหมายถูกแปลงจะแสดงขึ้นในรายการกล่องจดหมายที่ใช้ร่วมกันด้วย</span><span class="sxs-lookup"><span data-stu-id="0d3fa-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="0d3fa-p102">ถ้าคุณพยายามแปลงกล่องจดหมายในคอนโซลการดูแลอัตราแลกเปลี่ยน และการแปลงล้มเหลว ล้างแคชของเบราว์เซอร์และคุกกี้ของคุณ แล้วลองอีกครั้ง ถ้าจะยังคงทำงานไม่ได้ ลองแปลงกล่องจดหมายในเชลล์จัดการการแลกเปลี่ยน โดยการเรียกใช้คำสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0d3fa-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="0d3fa-107">ข้อมูลการแปลงกล่องจดหมายเพิ่มเติมจะพร้อมใช้งานในการ[แปลงเป็นกล่องจดหมายของผู้ใช้ไปยังกล่องจดหมายที่ใช้ร่วมกัน](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)</span><span class="sxs-lookup"><span data-stu-id="0d3fa-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
