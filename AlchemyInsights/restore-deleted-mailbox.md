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
ms.openlocfilehash: 14d2c9b1fe6764f5cd3a5a968586a19a03b62694
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641537"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="6cd43-102">คืนค่ากล่องจดหมายที่ถูกลบ</span><span class="sxs-lookup"><span data-stu-id="6cd43-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="6cd43-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply-re-assigning the license to the user.</span><span class="sxs-lookup"><span data-stu-id="6cd43-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
1. <span data-ttu-id="6cd43-104">ในศูนย์การจัดการ Microsoft 365 ให้ไปที่ **หน้า** \> **ผู้ใช้** ที่ใช้งานอยู่</span><span class="sxs-lookup"><span data-stu-id="6cd43-104">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="6cd43-105">เลือกผู้ใช้ในคําถาม</span><span class="sxs-lookup"><span data-stu-id="6cd43-105">Select the user in question.</span></span>

2. <span data-ttu-id="6cd43-106">บนแท็บ **สิทธิ์การใช้งานและแอป** ให้กําหนดสิทธิ์การใช้งาน Exchange Online แล้วเลือก **บันทึก** การเปลี่ยนแปลง</span><span class="sxs-lookup"><span data-stu-id="6cd43-106">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="6cd43-107">ถ้าคุณพยายามกู้คืนกล่องจดหมายที่แชร์หรือผู้ใช้ที่ถูกลบ กล่องจดหมายนั้นสามารถกู้คืนได้ภายใน 30 วัน</span><span class="sxs-lookup"><span data-stu-id="6cd43-107">If you are trying to recover a shared mailbox or a user that was deleted, it is also recoverable for 30 days.</span></span> <span data-ttu-id="6cd43-108">คุณสามารถค้นหาภายใต้ ผู้ใช้ \> **ที่ถูกลบ ผู้ใช้ ;** กล่องจดหมายที่แชร์ไม่ต้องใช้สิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="6cd43-108">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="6cd43-109">โปรดดูที่ [คืนค่า](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)ผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="6cd43-109">Please see [Restore a user](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="6cd43-110">การกู้คืนอีเมลจากกล่องจดหมายของผู้ใช้สามารถเสร็จสิ้นได้โดยผู้ดูแลระบบโดยไปที่ [ศูนย์การจัดการ Exchange](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353)ใหม่</span><span class="sxs-lookup"><span data-stu-id="6cd43-110">Recovery of email from user's mailbox can be done by admins by going to the [new Exchange Admin Center](https://techcommunity.microsoft.com/t5/exchange-team-blog/a-new-recoverableitems-experience-comes-to-exchange-online/ba-p/1505353).</span></span>

<span data-ttu-id="6cd43-111">สุดท้าย ถ้าคุณพยายามกู้คืนกล่องจดหมายที่ไม่ได้ใช้งาน ให้ปฏิบัติตาม [คําแนะนํา](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox)ที่นี่</span><span class="sxs-lookup"><span data-stu-id="6cd43-111">Finally, if you are trying to recover an Inactive mailbox, [follow the instructions here](https://docs.microsoft.com/microsoft-365/compliance/recover-an-inactive-mailbox).</span></span>
  
