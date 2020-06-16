---
title: เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้ Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749147"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="be8e9-102">เจ้าของไม่สามารถสร้างโฟลเดอร์ย่อยโดยใช้ Outlook</span><span class="sxs-lookup"><span data-stu-id="be8e9-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="be8e9-103">**มีปัญหาเกิดขึ้นกับเจ้าของโฟลเดอร์สาธารณะที่สร้างโฟลเดอร์ย่อยโดยใช้ Outlook ปัญหานี้จะได้รับการแก้ไขในเร็ว ๆ นี้**</span><span class="sxs-lookup"><span data-stu-id="be8e9-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="be8e9-104">ในขณะเดียวกัน ใช้หนึ่งในวิธีแก้ไขปัญหาต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="be8e9-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="be8e9-105">ใช้ Outlook สําหรับ MAC เพื่อสร้างโฟลเดอร์ย่อยเป็นปัญหาที่ส่งผลกระทบต่อ Outlook สําหรับหน้าต่างเดสก์ท็อปเท่านั้น (ทุกรุ่น)</span><span class="sxs-lookup"><span data-stu-id="be8e9-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="be8e9-106">ให้ผู้ดูแลระบบสร้างโฟลเดอร์ย่อยโดยใช้ EXO เชลล์หรือ EAC</span><span class="sxs-lookup"><span data-stu-id="be8e9-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="be8e9-107">การเปลี่ยนแปลงการDเริ่มต้นPublicFolderMailbox/EffectivePublicFolderMailboxบนกล่องจดหมายอื่นที่ไม่ใช่กล่องจดหมายเนื้อหาสําหรับโฟลเดอร์ที่ทําให้เกิดปัญหา</span><span class="sxs-lookup"><span data-stu-id="be8e9-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="be8e9-108">*ตั้งค่ากล่องจดหมายผู้ใช้1เริ่มต้น*</span><span class="sxs-lookup"><span data-stu-id="be8e9-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="be8e9-109">รอหนึ่งชั่วโมง เริ่มต้นไคลเอ็นต์ Outlook ใหม่</span><span class="sxs-lookup"><span data-stu-id="be8e9-109">Wait for an hour, restart outlook client</span></span>