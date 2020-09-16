---
title: คืนค่ากล่องจดหมายที่ถูกลบ
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
ms.openlocfilehash: 899eb7e171d125c509871c219f99dfd1106b858a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728090"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="8bd6b-102">การคืนค่ากล่องจดหมายที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="8bd6b-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="8bd6b-103">เมื่อผู้ใช้สูญเสียสิทธิ์การใช้งาน Exchange Online กล่องจดหมายของพวกเขาจะถูกเก็บไว้เป็นเวลา30วันและสามารถกู้คืนได้โดยเพียงแค่กำหนดสิทธิ์การใช้งานให้กับผู้ใช้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="8bd6b-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="8bd6b-104">*การดำเนินการนี้จะใช้งานได้ภายใน30วัน*</span><span class="sxs-lookup"><span data-stu-id="8bd6b-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="8bd6b-105">ในศูนย์การจัดการ Microsoft ๓๖๕ให้ไปที่**Users** \> หน้า**ผู้ใช้ที่ใช้งานอยู่**ของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="8bd6b-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="8bd6b-106">เลือกผู้ใช้ที่มีคำถาม</span><span class="sxs-lookup"><span data-stu-id="8bd6b-106">Select the user in question.</span></span>

2. <span data-ttu-id="8bd6b-107">บนแท็บสิทธิ์การใช้งาน**และแอป**ให้กำหนดสิทธิ์การใช้งาน Exchange Online และเลือก**บันทึกการเปลี่ยนแปลง**</span><span class="sxs-lookup"><span data-stu-id="8bd6b-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="8bd6b-108">ถ้าคุณกำลังพยายามกู้คืนกล่องจดหมายที่แชร์คุณจะได้รับการกู้คืนเป็นเวลา30วัน</span><span class="sxs-lookup"><span data-stu-id="8bd6b-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="8bd6b-109">คุณสามารถค้นหาบุคคลเหล่านั้นได้ภายใต้ **ผู้**ใช้ที่ \> **ถูกลบผู้ใช้**กล่องจดหมายที่แชร์ไม่จำเป็นต้องมีสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="8bd6b-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="8bd6b-110">ถ้าคุณทราบว่าคุณต้องการคืนค่าผู้ใช้ที่ถูกลบโปรดดู[คืนค่าผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="8bd6b-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
  