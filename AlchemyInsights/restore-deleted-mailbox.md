---
title: การคืนค่ากล่องจดหมายที่ถูกลบ
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
ms.openlocfilehash: 18e56305b60469422a154ffa1b097c238baaae16
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764675"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="32a70-102">การคืนค่ากล่องจดหมายที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="32a70-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="32a70-103">เมื่อผู้ใช้สูญเสียสิทธิ์การใช้งาน Exchange แบบออนไลน์ กล่องจดหมายของพวกเขาจะถูกเก็บไว้สําหรับ 30 วัน และสามารถกู้คืน โดยเพียง re-assigning สิทธิ์การใช้งานให้กับผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="32a70-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="32a70-104">*นี้จะทํางานภายใน 30 วัน.*</span><span class="sxs-lookup"><span data-stu-id="32a70-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="32a70-105">ในศูนย์การจัดการ Microsoft 365 ไปที่เพจ**ผู้ใช้**\>**ที่ใช้งานอยู่**</span><span class="sxs-lookup"><span data-stu-id="32a70-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="32a70-106">เลือกผู้ใช้ที่ต้องการ</span><span class="sxs-lookup"><span data-stu-id="32a70-106">Select the user in question.</span></span>

2. <span data-ttu-id="32a70-107">บนแท็บ**สิทธิ์การใช้งานและแอป**ให้กําหนดสิทธิ์การใช้งาน Exchange Online แล้วเลือก**บันทึกการเปลี่ยนแปลง**</span><span class="sxs-lookup"><span data-stu-id="32a70-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="32a70-108">ถ้าคุณกําลังพยายามกู้คืนกล่องจดหมายที่ใช้ร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="32a70-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="32a70-109">คุณสามารถค้นหาได้ภายใต้**ผู้ใช้**\>**ที่ถูกลบ** กล่องจดหมายที่ใช้ร่วมกันไม่จําเป็นต้องมีใบอนุญาต</span><span class="sxs-lookup"><span data-stu-id="32a70-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="32a70-110">ถ้าคุณตระหนักว่าคุณจําเป็นต้องคืนค่าผู้ใช้ที่ถูกลบโปรดดู[การคืนค่าผู้ใช้](https://docs.microsoft.com/office365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="32a70-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  