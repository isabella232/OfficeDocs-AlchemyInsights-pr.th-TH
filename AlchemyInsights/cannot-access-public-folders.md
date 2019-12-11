---
title: ไม่สามารถเข้าถึงโฟลเดอร์สาธารณะ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959513"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="14767-102">Outlook ไม่สามารถเชื่อมต่อไปยังโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="14767-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="14767-103">ถ้าการเข้าถึงโฟลเดอร์สาธารณะไม่ทำงานสำหรับผู้ใช้ไม่กี่ให้ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="14767-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="14767-104">เชื่อมต่อกับ EXO PowerShell และกำหนดค่าการ DefaultPublicFolderMailbox จดหมายบนบัญชีผู้ใช้ที่มีปัญหาเพื่อให้ตรงกับหนึ่งในบัญชีผู้ใช้ที่ทำงาน</span><span class="sxs-lookup"><span data-stu-id="14767-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="14767-105">ตัว อย่าง เช่น:</span><span class="sxs-lookup"><span data-stu-id="14767-105">Example:</span></span>

<span data-ttu-id="14767-106">ได้รับกล่องจดหมายผู้ใช้ , EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="14767-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="14767-107">กล่องจดหมาย ProblemUser \<ค่าจากคำสั่งก่อนหน้านี้></span><span class="sxs-lookup"><span data-stu-id="14767-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="14767-108">รออย่างน้อยหนึ่งชั่วโมงสำหรับการเปลี่ยนแปลงมีผลบังคับใช้</span><span class="sxs-lookup"><span data-stu-id="14767-108">Wait at least one hour for the change to take effect.</span></span>