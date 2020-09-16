---
title: เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft ๓๖๕
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
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733706"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="95d0d-102">เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="95d0d-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="95d0d-103">คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft ๓๖๕โดยใช้ศูนย์การจัดการ</span><span class="sxs-lookup"><span data-stu-id="95d0d-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="95d0d-104">เพียงเลือกกลุ่มแล้วเลือก @edit อีเมลแอดเดรส</span><span class="sxs-lookup"><span data-stu-id="95d0d-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="95d0d-105">นอกจากนี้คุณยังสามารถใช้คำสั่ง EXO PowerShell เพื่อเปลี่ยนที่อยู่ SMTP หลักของกลุ่ม Microsoft ๓๖๕ได้ดังนี้</span><span class="sxs-lookup"><span data-stu-id="95d0d-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="95d0d-106">ตั้งค่า-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="95d0d-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="95d0d-107">ตัวอย่าง</span><span class="sxs-lookup"><span data-stu-id="95d0d-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
