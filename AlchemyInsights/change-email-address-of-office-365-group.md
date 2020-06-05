---
title: เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580676"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="58ec0-102">เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="58ec0-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="58ec0-103">คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365 โดยใช้ศูนย์การจัดการ</span><span class="sxs-lookup"><span data-stu-id="58ec0-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="58ec0-104">เพียงเลือกกลุ่มและเลือกที่อยู่อีเมล@edit</span><span class="sxs-lookup"><span data-stu-id="58ec0-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="58ec0-105">คุณยังสามารถใช้คําสั่งต่อไปนี้คําสั่ง EXO PowerShell เพื่อเปลี่ยนอยู่ SMTP หลักของกลุ่ม Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="58ec0-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="58ec0-106">ชุดรวมกลุ่ม <Group Name> -หลักSmtpที่อยู่<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="58ec0-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="58ec0-107">ตัว อย่าง เช่น:</span><span class="sxs-lookup"><span data-stu-id="58ec0-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
