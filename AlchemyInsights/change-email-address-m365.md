---
title: เปลี่ยนที่อยู่อีเมลของ Microsoft ๓๖๕กลุ่ม
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
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/10/2020
ms.locfileid: "48462059"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="2cf98-102">เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="2cf98-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="2cf98-103">คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft ๓๖๕โดยใช้ศูนย์การจัดการ</span><span class="sxs-lookup"><span data-stu-id="2cf98-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="2cf98-104">เพียงเลือกกลุ่มแล้วเลือก @edit อีเมลแอดเดรส</span><span class="sxs-lookup"><span data-stu-id="2cf98-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="2cf98-105">นอกจากนี้คุณยังสามารถใช้คำสั่ง EXO PowerShell เพื่อเปลี่ยนที่อยู่ SMTP หลักของกลุ่ม Microsoft ๓๖๕ได้ดังนี้</span><span class="sxs-lookup"><span data-stu-id="2cf98-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="2cf98-106">ตัวอย่าง</span><span class="sxs-lookup"><span data-stu-id="2cf98-106">Example:</span></span>

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
