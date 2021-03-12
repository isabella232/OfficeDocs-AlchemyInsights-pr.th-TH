---
title: แก้ไขการตั้งค่านโยบาย/กล่องจดหมายของผู้ใช้
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750565"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="2fdfa-102">แก้ไขการตั้งค่านโยบาย/กล่องจดหมายของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="2fdfa-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="2fdfa-103">การตั้งค่าอีเมลขยะบนกล่องจดหมายมีผลต่อข้อความนี้</span><span class="sxs-lookup"><span data-stu-id="2fdfa-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="2fdfa-104">เมื่อต้องการรีวิวการตั้งค่า ให้ทต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="2fdfa-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="2fdfa-105">เปิดใช้ Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="2fdfa-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="2fdfa-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="2fdfa-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="2fdfa-107">เรียกใช้การสั่งนี้ (โดยใช้ที่อยู่อีเมลของผู้ใช้):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="2fdfa-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="2fdfa-108">ตรวจสอบว่าที่อยู่อีเมลของผู้ส่งเป็นส่วนหนึ่งของ **TrustedSendersAndDomains** หรือ **BlockedSendersAndDomains** หรือไม่</span><span class="sxs-lookup"><span data-stu-id="2fdfa-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="2fdfa-109">ถ้าที่อยู่อีเมลอยู่ในรายการใดรายการหนึ่ง คุณอาจต้องลบออก</span><span class="sxs-lookup"><span data-stu-id="2fdfa-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="2fdfa-110">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[Set-MailboxJunkAmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047)</span><span class="sxs-lookup"><span data-stu-id="2fdfa-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
