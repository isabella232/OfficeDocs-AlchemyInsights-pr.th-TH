---
title: เปลี่ยนที่อยู่อีเมลของ Microsoft ๓๖๕กลุ่มหรือทีม Microsoft
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756576"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="f26a4-102">เปลี่ยนที่อยู่อีเมลของ Microsoft ๓๖๕กลุ่มหรือทีม Microsoft</span><span class="sxs-lookup"><span data-stu-id="f26a4-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="f26a4-103">คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft ๓๖๕หรือทีม Microsoft ได้โดยใช้[ศูนย์การจัดการ Microsoft ๓๖๕](https://admin.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="f26a4-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="f26a4-104">เพียงเลือกกลุ่มแล้วเลือก @edit อีเมลแอดเดรส</span><span class="sxs-lookup"><span data-stu-id="f26a4-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="f26a4-105">คุณยังสามารถใช้คำสั่ง EXO PowerShell ต่อไปนี้เพื่อเปลี่ยนที่อยู่ SMTP หลักของกลุ่ม/ทีม Microsoft ๓๖๕:</span><span class="sxs-lookup"><span data-stu-id="f26a4-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="f26a4-106">ตัวอย่าง</span><span class="sxs-lookup"><span data-stu-id="f26a4-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
