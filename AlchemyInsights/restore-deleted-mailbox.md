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
ms.openlocfilehash: 284024bdf9728e8463fe69ef9c9c2695035faf2f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511383"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="fcec3-102">การคืนค่ากล่องจดหมายที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="fcec3-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="fcec3-103">เมื่อผู้ใช้สูญเสียสิทธิ์การใช้งาน Exchange แบบออนไลน์ กล่องจดหมายของพวกเขาจะถูกเก็บไว้ 30 วัน และสามารถกู้คืน โดยเพียง re-assigning สิทธิ์การใช้งานสําหรับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="fcec3-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="fcec3-104">*นี้จะทํางานภายใน 30 วันเท่านั้น*</span><span class="sxs-lookup"><span data-stu-id="fcec3-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="fcec3-105">ในศูนย์การจัดการ Microsoft 365 ให้ไปที่หน้า**Users** \> **ผู้ใช้ที่ใช้งานอยู่**</span><span class="sxs-lookup"><span data-stu-id="fcec3-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="fcec3-106">เลือกผู้ใช้ที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="fcec3-106">Select the user in question.</span></span>

2. <span data-ttu-id="fcec3-107">บนแท็บ**สิทธิ์การใช้งานและแอป**ให้กําหนดสิทธิ์การใช้งาน Exchange Online แล้วเลือก**บันทึกการเปลี่ยนแปลง**</span><span class="sxs-lookup"><span data-stu-id="fcec3-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="fcec3-108">ถ้าคุณกําลังพยายามกู้คืนกล่องจดหมายที่ใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="fcec3-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="fcec3-109">คุณสามารถค้นหาได้ภายใต้**Users** \> **ผู้ใช้ที่ถูกลบ**; กล่องจดหมายที่ใช้ร่วมกันไม่จําเป็นต้องมีสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="fcec3-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="fcec3-110">ถ้าคุณทราบว่าคุณต้องคืนค่าผู้ใช้ที่ถูกลบไปแล้ว โปรดดู[การคืนค่าผู้ใช้](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="fcec3-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
  