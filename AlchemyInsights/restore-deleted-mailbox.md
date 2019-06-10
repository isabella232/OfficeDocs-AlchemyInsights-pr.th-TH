---
title: กล่องจดหมายการคืนค่าลบ
ms.author: pebaum
author: pebaum
ms.date: 9/12/2017
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 760587c0e58662283c3c1a647d1cc5fb81187545
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770757"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="b34ec-102">การคืนค่ากล่องจดหมายถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="b34ec-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="b34ec-103">เมื่อผู้ใช้สูญเสียสิทธิ์การใช้งานการแลกเปลี่ยนแบบออนไลน์ กล่องจดหมายของพวกเขาจะถูกเก็บไว้สำหรับ 30 วัน และสามารถถูกกู้คืน โดยเพียงแค่อีกครั้งกำหนดสิทธิ์การใช้งานสำหรับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="b34ec-103">When the user loses its Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="b34ec-104">*ซึ่งจะทำงานภายใน 30 วันเท่านั้น*</span><span class="sxs-lookup"><span data-stu-id="b34ec-104">*This will work only within 30 days.*</span></span>  <span data-ttu-id="b34ec-105">ในพอร์ทัล Admin ไปที่:</span><span class="sxs-lookup"><span data-stu-id="b34ec-105">In the Admin Portal, go to:</span></span> 
  
1. <span data-ttu-id="b34ec-106">**ผู้ใช้** \>ผู้ใช้**ที่ใช้งานอยู่**</span><span class="sxs-lookup"><span data-stu-id="b34ec-106">**Users** \> **Active** users.</span></span> <span data-ttu-id="b34ec-107">เลือกผู้ใช้สงสัย</span><span class="sxs-lookup"><span data-stu-id="b34ec-107">Select the user in question.</span></span> 
    
2. <span data-ttu-id="b34ec-108">กด**แก้ไข**เพื่อปรับเปลี่ยนสิทธิ์การใช้งานผลิตภัณฑ์</span><span class="sxs-lookup"><span data-stu-id="b34ec-108">Press **Edit** to modify Product licenses</span></span> 
    
3. <span data-ttu-id="b34ec-109">กำหนดสิทธิ์การใช้งานแบบออนไลน์ของอัตราแลกเปลี่ยน และกด**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="b34ec-109">Assign the Exchange Online license and press **Save**</span></span>
    
<span data-ttu-id="b34ec-110">ถ้าคุณกำลังพยายามกู้คืนกล่องจดหมายที่ใช้ร่วมกัน ได้นอกจากนี้ยังได้รับคืนสำหรับ 30 วัน</span><span class="sxs-lookup"><span data-stu-id="b34ec-110">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="b34ec-111">คุณสามารถค้นหาได้ภายใต้**ผู้ใช้**\>ผู้ใช้**ถูกลบ** กล่องจดหมายที่ใช้ร่วมกันไม่จำเป็นต้องมีสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="b34ec-111">You can find them under **Users** \> **Deleted** users; shared mailboxes do not require a license.</span></span> <span data-ttu-id="b34ec-112">ถ้าคุณรับรู้ว่า คุณจำเป็นต้องคืนค่าผู้ใช้ถูกลบไปแล้ว โปรดดู[ผู้ใช้ใน Office 365 การคืนค่า](https://docs.microsoft.com/office365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="b34ec-112">If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  

