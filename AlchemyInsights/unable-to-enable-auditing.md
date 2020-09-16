---
title: ๒๔๑๙-ไม่สามารถเปิดใช้งาน-การตรวจสอบ
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767618"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="0b2ef-102">ไม่สามารถเปิดใช้งานการตรวจสอบแบบรวมได้</span><span class="sxs-lookup"><span data-stu-id="0b2ef-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="0b2ef-103">เมื่อคุณพยายามเปิดใช้งานการตรวจสอบแบบรวมสำหรับองค์กรของคุณคุณอาจได้รับข้อผิดพลาดคล้ายกับต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0b2ef-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="0b2ef-104">เมื่อต้องการแก้ไขปัญหานี้ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0b2ef-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="0b2ef-105">[เชื่อมต่อกับ Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="0b2ef-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="0b2ef-106">เรียกใช้ cmdlet ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0b2ef-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="0b2ef-107">รอ๖๐นาทีสำหรับการตั้งค่าก่อนหน้านี้จะมีผล</span><span class="sxs-lookup"><span data-stu-id="0b2ef-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="0b2ef-108">เรียกใช้คำสั่งต่อไปนี้ใน Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="0b2ef-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="0b2ef-109">สำหรับข้อมูลเพิ่มเติมให้ดูบทความต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0b2ef-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="0b2ef-110">เชื่อมต่อกับ Exchange Online PowerShell โดยใช้การรับรองความถูกต้องแบบหลายปัจจัย</span><span class="sxs-lookup"><span data-stu-id="0b2ef-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="0b2ef-111">เปิดหรือปิดการค้นหาบันทึกการตรวจสอบ</span><span class="sxs-lookup"><span data-stu-id="0b2ef-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
