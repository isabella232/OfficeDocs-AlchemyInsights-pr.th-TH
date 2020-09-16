---
title: ๑๓๗๔แก้ไข howto กล่องจดหมายที่สอง
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1374"
- "2692"
- "3500014"
ms.assetid: 8bf1a8f2-58ef-4697-b9c0-be340de96bfe
ms.openlocfilehash: 048c527b26d138535550b5bae399d0ce9fbce0a6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720917"
---
# <a name="a-user-has-two-mailboxes"></a><span data-ttu-id="54de7-102">ผู้ใช้มีกล่องจดหมายสองกล่อง</span><span class="sxs-lookup"><span data-stu-id="54de7-102">A user has two mailboxes</span></span>

<span data-ttu-id="54de7-103">สภาพแวดล้อมแบบไฮบริดที่ใช้ Azure Active Directory Connect (AAD Connect) หรือ DirSync อาจทำให้ผู้ใช้มีกล่องจดหมายสองกล่องดังต่อไปนี้: หนึ่งในองค์กรและหนึ่งในระบบคลาวด์</span><span class="sxs-lookup"><span data-stu-id="54de7-103">Hybrid environments that use Azure Active Directory Connect (AAD Connect) or DirSync might accidentally cause a user to have two mailboxes: one on-premises, and one in the cloud.</span></span> <span data-ttu-id="54de7-104">ไม่สามารถสร้างกล่องจดหมายที่ซ้ำกันได้ในที่ใดที่หนึ่ง</span><span class="sxs-lookup"><span data-stu-id="54de7-104">A duplicate mailbox could be created in either place.</span></span>

<span data-ttu-id="54de7-105">เมื่อต้องการแก้ไขปัญหานี้ให้ดู[วิธีการกู้คืนเมื่อมีกล่องจดหมายที่มีอยู่ทั้งใน Exchange Online และภายในองค์กร](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises)</span><span class="sxs-lookup"><span data-stu-id="54de7-105">To resolve this issue, see [How to recover when a mailbox exists in both Exchange Online and on-premises](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises).</span></span> <span data-ttu-id="54de7-106">ถ้าคุณต้องการเรียนรู้เพิ่มเติมเกี่ยวกับวิธีการหลีกเลี่ยงปัญหานี้เกิดขึ้นในอนาคตให้ดู[ที่ผู้ใช้ของฉันมีกล่องจดหมายทั้งภายในองค์กรและใน Exchange Online วิธีใช้!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809)</span><span class="sxs-lookup"><span data-stu-id="54de7-106">If you want to learn more about how to avoid this from happening in the future, see [My user has a mailbox both on-premises and in Exchange Online. Help!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).</span></span>
