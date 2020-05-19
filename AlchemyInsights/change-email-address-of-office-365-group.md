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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283263"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="0cc20-102">เปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0cc20-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="0cc20-103">คุณสามารถเปลี่ยนที่อยู่อีเมลของกลุ่ม Microsoft 365 โดยใช้ศูนย์การจัดการ</span><span class="sxs-lookup"><span data-stu-id="0cc20-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="0cc20-104">เพียงเลือกกลุ่มและเลือกที่อยู่อีเมล@edit</span><span class="sxs-lookup"><span data-stu-id="0cc20-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="0cc20-105">คุณยังสามารถใช้ต่อไปนี้คําสั่ง PowerShell EXO เพื่อเปลี่ยนอยู่ SMTP หลักของกลุ่ม Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="0cc20-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="0cc20-106">ตั้งค่า-รวมกลุ่ม <Group Name> -หลักที่อยู่<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="0cc20-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="0cc20-107">ตัว อย่าง เช่น:</span><span class="sxs-lookup"><span data-stu-id="0cc20-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
