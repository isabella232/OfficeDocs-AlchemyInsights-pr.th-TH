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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891768"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="28763-102">Outlook ไม่สามารถเชื่อมต่อกับโฟลเดอร์สาธารณะ</span><span class="sxs-lookup"><span data-stu-id="28763-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="28763-103">ถ้าการเข้าถึงโฟลเดอร์สาธารณะไม่ทํางานสําหรับผู้ใช้บางราย ให้ลองทําดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="28763-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="28763-104">เชื่อมต่อกับ POWERShell EXO และกําหนดค่าพารามิเตอร์ DefaultPublicFolderMailbox ในบัญชีผู้ใช้ปัญหาให้ตรงกับพารามิเตอร์ในบัญชีผู้ใช้ที่ทํางาน</span><span class="sxs-lookup"><span data-stu-id="28763-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="28763-105">ตัว อย่าง เช่น:</span><span class="sxs-lookup"><span data-stu-id="28763-105">Example:</span></span>

<span data-ttu-id="28763-106">รับกล่องจดหมายทํางานผู้ใช้ | ฟุตเริ่มต้นโฟลเดอร์สาธารณะกล่องจดหมาย, ที่มีประสิทธิภาพสาธารณะโฟลเดอร์กล่องจดหมาย</span><span class="sxs-lookup"><span data-stu-id="28763-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="28763-107">ตั้งค่ากล่องจดหมายปัญหาผู้ใช้ -DefaultPublicFolderกล่องจดหมาย\<ค่าจากคําสั่งก่อนหน้านี้></span><span class="sxs-lookup"><span data-stu-id="28763-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="28763-108">รออย่างน้อยหนึ่งชั่วโมงเพื่อให้การเปลี่ยนแปลงมีผล</span><span class="sxs-lookup"><span data-stu-id="28763-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="28763-109">ถ้าปัญหายังคงอยู่ โปรดทําตามขั้นตอน[นี้เพื่อ](https://aka.ms/pfcte)แก้ไขปัญหาการเข้าถึงโฟลเดอร์สาธารณะโดยใช้ Outlook</span><span class="sxs-lookup"><span data-stu-id="28763-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>