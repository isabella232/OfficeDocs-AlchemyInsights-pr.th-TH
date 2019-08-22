---
title: แปลงกล่องจดหมายของผู้ใช้ลงในกล่องจดหมายที่ใช้ร่วมกันได้อย่างไร
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496454"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="97f55-102">แปลงเป็นกล่องจดหมายของผู้ใช้ลงในกล่องจดหมายที่ใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="97f55-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="97f55-103">คุณสามารถแปลงได้เฉพาะกล่องจดหมายของผู้ใช้ไปยังกล่องจดหมายที่ใช้ร่วมกันถ้าผู้ใช้มีสิทธิ์การใช้งานของการแลกเปลี่ยน</span><span class="sxs-lookup"><span data-stu-id="97f55-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="97f55-104">หลังจากกล่องจดหมายจะถูกแปลง จะยังคงแสดงอยู่ในรายการผู้ใช้ที่ใช้งานอยู่ได้เนื่องจากรายการที่มีกล่องจดหมายที่ใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="97f55-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="97f55-105">อย่างไรก็ตาม กล่องจดหมายถูกแปลงจะแสดงขึ้นในรายการกล่องจดหมายที่ใช้ร่วมกันด้วย</span><span class="sxs-lookup"><span data-stu-id="97f55-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="97f55-106">ถ้าคุณพยายามแปลงกล่องจดหมายในคอนโซลการดูแลอัตราแลกเปลี่ยน และการแปลงล้มเหลว ล้างแคชของเบราว์เซอร์และคุกกี้ของคุณ แล้วลองอีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="97f55-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="97f55-107">ถ้าจะยังคงทำงานไม่ได้ ลองแปลงกล่องจดหมายในเชลล์จัดการการแลกเปลี่ยน โดยการเรียกใช้คำสั่งต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="97f55-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="97f55-108">ข้อมูลการแปลงกล่องจดหมายเพิ่มเติมจะพร้อมใช้งานในการ[แปลงเป็นกล่องจดหมายของผู้ใช้ไปยังกล่องจดหมายที่ใช้ร่วมกัน](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox)</span><span class="sxs-lookup"><span data-stu-id="97f55-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
