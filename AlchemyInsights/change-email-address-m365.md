---
title: เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365 หรือ Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819099"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a><span data-ttu-id="ea349-102">เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365 หรือ Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ea349-102">Change email address of a Microsoft 365 group or Microsoft Teams</span></span>

<span data-ttu-id="ea349-103">คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365 หรือ Microsoft Teams โดยใช้ศูนย์การจัดการ[Microsoft 365](https://admin.microsoft.com/)</span><span class="sxs-lookup"><span data-stu-id="ea349-103">You can change the email address of a Microsoft 365 group or Microsoft Teams by using the [Microsoft 365 admin center](https://admin.microsoft.com/).</span></span> <span data-ttu-id="ea349-104">เพียงเลือกกลุ่ม @editที่อยู่อีเมลของคุณ</span><span class="sxs-lookup"><span data-stu-id="ea349-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="ea349-105">คุณยังสามารถใช้สั่ง EXO PowerShell ต่อไปนี้เพื่อเปลี่ยนที่อยู่ SMTP หลักของกลุ่ม Microsoft 365/Teams:</span><span class="sxs-lookup"><span data-stu-id="ea349-105">You can also use the following EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group/Teams:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="ea349-106">ตัวอย่าง:</span><span class="sxs-lookup"><span data-stu-id="ea349-106">Example:</span></span>

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
