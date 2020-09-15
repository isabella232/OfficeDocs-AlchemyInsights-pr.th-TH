---
title: เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้ Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665737"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="92c72-102">เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้ Outlook</span><span class="sxs-lookup"><span data-stu-id="92c72-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="92c72-103">**มีปัญหาที่เกิดขึ้นอย่างต่อเนื่องกับเจ้าของโฟลเดอร์สาธารณะการสร้างโฟลเดอร์ย่อยโดยใช้ Outlook ปัญหานี้จะได้รับการแก้ไขในเร็วๆนี้**</span><span class="sxs-lookup"><span data-stu-id="92c72-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="92c72-104">ในขณะเดียวกันให้ใช้หนึ่งในวิธีการแก้ไขปัญหาต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="92c72-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="92c72-105">ใช้ Outlook for MAC เพื่อสร้างโฟลเดอร์ย่อยเป็นปัญหาที่มีผลต่อ Outlook สำหรับเดสก์ท็อป windows (ทุกเวอร์ชัน)</span><span class="sxs-lookup"><span data-stu-id="92c72-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="92c72-106">มีผู้ดูแลระบบสร้างโฟลเดอร์ย่อยโดยใช้ Shell หรือ EAC</span><span class="sxs-lookup"><span data-stu-id="92c72-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="92c72-107">เปลี่ยน DefaultPublicFolderMailbox/EffectivePublicFolderMailbox บนผู้ใช้ไปยังกล่องจดหมายอื่นที่ไม่ใช่กล่องจดหมายเนื้อหาสำหรับโฟลเดอร์ที่ทำให้เกิดปัญหา</span><span class="sxs-lookup"><span data-stu-id="92c72-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="92c72-108">*ตั้งค่ากล่องจดหมาย User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="92c72-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="92c72-109">รอสักครู่ให้เริ่มไคลเอ็นต์ outlook ใหม่</span><span class="sxs-lookup"><span data-stu-id="92c72-109">Wait for an hour, restart outlook client</span></span>