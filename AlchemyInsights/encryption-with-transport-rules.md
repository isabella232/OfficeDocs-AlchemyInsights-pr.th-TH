---
title: การเข้ารหัสลับที่มีกฎการขนส่ง
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
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784362"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="ba1b1-102">การเข้ารหัสลับที่มีกฎการขนส่ง</span><span class="sxs-lookup"><span data-stu-id="ba1b1-102">Encryption with transport rules</span></span>

<span data-ttu-id="ba1b1-103">ใน [ศูนย์การจัดการ Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) คุณสามารถใช้ความสามารถในการเข้ารหัสลับข้อความของ OFFICE (OME) ในกฎโฟลว์จดหมายของคุณเพื่อทริกเกอร์การเข้ารหัสลับข้อความ</span><span class="sxs-lookup"><span data-stu-id="ba1b1-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="ba1b1-104">เลือกตัวเลือกการ **ใช้การเข้ารหัสลับข้อความของ Office ๓๖๕และการป้องกันสิทธิ์** บนเงื่อนไขของกฎการขนส่ง</span><span class="sxs-lookup"><span data-stu-id="ba1b1-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="ba1b1-105">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่กำหนดกฎโฟลว์จดหมายเพื่อเข้ารหัสลับ](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="ba1b1-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="ba1b1-106">ใน Powershell ให้ใช้ cmdlet [TransportRule ใหม่](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) และตั้งค่าพารามิเตอร์ *ApplyOME* เป็น $true</span><span class="sxs-lookup"><span data-stu-id="ba1b1-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>
