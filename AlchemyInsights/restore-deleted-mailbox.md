---
title: กล่องจดหมายการคืนค่าลบ
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 44b23be5e75a0669821bbeb07b0f064eeef6d021
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666391"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="07108-102">การคืนค่ากล่องจดหมายถูกลบไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="07108-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="07108-103">เมื่อผู้ใช้สูญเสียสิทธิ์การใช้งานการแลกเปลี่ยนแบบออนไลน์ กล่องจดหมายของพวกเขาจะถูกเก็บไว้สำหรับ 30 วัน และสามารถถูกกู้คืน โดยเพียงแค่อีกครั้งกำหนดสิทธิ์การใช้งานสำหรับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="07108-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="07108-104">*ซึ่งจะทำงานภายใน 30 วันเท่านั้น*</span><span class="sxs-lookup"><span data-stu-id="07108-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="07108-105">ใน Microsoft 365 admin ศูนย์ ไปยัง**ผู้ใช้**\>หน้า**ผู้ใช้ที่ใช้งานอยู่**</span><span class="sxs-lookup"><span data-stu-id="07108-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="07108-106">เลือกผู้ใช้สงสัย</span><span class="sxs-lookup"><span data-stu-id="07108-106">Select the user in question.</span></span>

2. <span data-ttu-id="07108-107">บนแท็บของ**สิทธิ์การใช้งานและโปรแกรมประยุกต์**กำหนดสิทธิ์การใช้งานแบบออนไลน์ของอัตราแลกเปลี่ยน และเลือก**บันทึกการเปลี่ยนแปลง**</span><span class="sxs-lookup"><span data-stu-id="07108-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="07108-108">ถ้าคุณกำลังพยายามกู้คืนกล่องจดหมายที่ใช้ร่วมกัน ได้นอกจากนี้ยังได้รับคืนสำหรับ 30 วัน</span><span class="sxs-lookup"><span data-stu-id="07108-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="07108-109">คุณสามารถค้นหาได้ภายใต้**ผู้ใช้** \> **ผู้ใช้ถูกลบ** กล่องจดหมายที่ใช้ร่วมกันไม่จำเป็นต้องมีสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="07108-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="07108-110">ถ้าคุณรับรู้ว่า คุณจำเป็นต้องคืนค่าผู้ใช้ถูกลบไปแล้ว โปรดดู[ผู้ใช้ใน Office 365 การคืนค่า](https://docs.microsoft.com/office365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="07108-110">If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  