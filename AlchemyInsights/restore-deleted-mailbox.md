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
ms.custom: Adm_O365
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: f9529dc92637e6b6174ff3cb8d1587ab2dffd0e2
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29927523"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="480ec-102">การคืนค่ากล่องจดหมายถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="480ec-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="480ec-103">เมื่อผู้ใช้สูญเสียสิทธิ์การใช้งานการแลกเปลี่ยนแบบออนไลน์ กล่องจดหมายของพวกเขาจะถูกเก็บไว้สำหรับ 30 วัน และสามารถถูกกู้คืน โดยเพียงแค่อีกครั้งกำหนดสิทธิ์การใช้งานสำหรับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="480ec-103">When the user loses its Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="480ec-p101">*นี้จะใช้ได้เฉพาะภายใน 30 วัน*  ในพอร์ทัล Admin ไปที่:</span><span class="sxs-lookup"><span data-stu-id="480ec-p101">*This will work only within 30 days.*  In the Admin Portal, go to:</span></span> 
  
1. <span data-ttu-id="480ec-p102">**ผู้ใช้** \>ผู้ใช้**ที่ใช้งานอยู่** เลือกผู้ใช้สงสัย</span><span class="sxs-lookup"><span data-stu-id="480ec-p102">**Users** \> **Active** users. Select the user in question.</span></span> 
    
2. <span data-ttu-id="480ec-108">กด**แก้ไข**เพื่อปรับเปลี่ยนสิทธิ์การใช้งานผลิตภัณฑ์</span><span class="sxs-lookup"><span data-stu-id="480ec-108">Press **Edit** to modify Product licenses</span></span> 
    
3. <span data-ttu-id="480ec-109">กำหนดสิทธิ์การใช้งานแบบออนไลน์ของอัตราแลกเปลี่ยน และกด**บันทึก**</span><span class="sxs-lookup"><span data-stu-id="480ec-109">Assign the Exchange Online license and press **Save**</span></span>
    
<span data-ttu-id="480ec-p103">ถ้าคุณกำลังพยายามกู้คืนกล่องจดหมายที่ใช้ร่วมกัน ได้นอกจากนี้ยังได้รับคืนสำหรับ 30 วัน คุณสามารถค้นหาได้ภายใต้**ผู้ใช้**\>ผู้ใช้ที่**ถูกลบ**ได้ กล่องจดหมายที่ใช้ร่วมกันไม่จำเป็นต้องมีสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="480ec-p103">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days. You can find them under **Users** \> **Deleted** users. Shared mailboxes do not require a license.</span></span> 
  

