---
title: เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้ Outlook ได้
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836154"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="2a6d4-102">เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้ Outlook ได้</span><span class="sxs-lookup"><span data-stu-id="2a6d4-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="2a6d4-103">**มีปัญหาที่เจ้าของโฟลเดอร์สาธารณะสร้างโฟลเดอร์ย่อยโดยใช้ Outlook อย่างต่อเนื่อง ปัญหานี้จะได้รับการแก้ไขในเร็วๆ นี้**</span><span class="sxs-lookup"><span data-stu-id="2a6d4-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="2a6d4-104">ขณะเดียวกัน ให้ใช้วิธีแก้ไขปัญหาชั่วคราวข้อใดข้อหนึ่งต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="2a6d4-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="2a6d4-105">ใช้ Outlook for MAC เพื่อสร้างโฟลเดอร์ย่อยเนื่องจากปัญหาส่งผลกระทบต่อ Outlook for Windows บนเดสก์ท็อปเท่านั้น (ทุกเวอร์ชัน)</span><span class="sxs-lookup"><span data-stu-id="2a6d4-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="2a6d4-106">ให้ผู้ดูแลระบบสร้างโฟลเดอร์ย่อยโดยใช้ EXO Shell หรือ EAC</span><span class="sxs-lookup"><span data-stu-id="2a6d4-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="2a6d4-107">เปลี่ยน DefaultPublicFolderMailbox/EffectivePublicFolderMailbox บนผู้ใช้เป็นกล่องจดหมายอื่นนอกเหนือจากกล่องจดหมายเนื้อหาของโฟลเดอร์ที่ทําให้เกิดปัญหา</span><span class="sxs-lookup"><span data-stu-id="2a6d4-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="2a6d4-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="2a6d4-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="2a6d4-109">รอหนึ่งชั่วโมง รีสตาร์ตไคลเอ็นต์ Outlook</span><span class="sxs-lookup"><span data-stu-id="2a6d4-109">Wait for an hour, restart outlook client</span></span>