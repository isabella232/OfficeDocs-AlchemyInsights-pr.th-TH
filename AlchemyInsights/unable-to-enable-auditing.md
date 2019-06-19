---
title: 2419-ไม่การเปิดใช้งานการตรวจสอบ
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065717"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="13edb-102">ไม่สามารถเปิดใช้งานการตรวจสอบประกอบการ</span><span class="sxs-lookup"><span data-stu-id="13edb-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="13edb-103">เมื่อคุณพยายามที่จะเปิดใช้งานการตรวจสอบสำหรับองค์กรของคุณ Office 365 ประกอบการ คุณอาจได้รับข้อผิดพลาดที่คล้ายคลึงกันต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="13edb-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="13edb-104">เมื่อต้องการแก้ไขปัญหานี้ ให้ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="13edb-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="13edb-105">การ[เชื่อมต่อการแลกเปลี่ยน Powershell แบบออนไลน์](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)</span><span class="sxs-lookup"><span data-stu-id="13edb-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="13edb-106">เรียกใช้ cmdlet ต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="13edb-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="13edb-107">รอ 60 นาทีสำหรับการตั้งค่าก่อนหน้านี้มีผลบังคับใช้</span><span class="sxs-lookup"><span data-stu-id="13edb-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="13edb-108">เรียกใช้คำสั่งต่อไปนี้ใน PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน:</span><span class="sxs-lookup"><span data-stu-id="13edb-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="13edb-109">สำหรับข้อมูลเพิ่มเติม ดูบทความต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="13edb-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="13edb-110">เชื่อมต่อกับ Exchange PowerShell แบบออนไลน์โดยใช้การรับรองความถูกต้องด้วยหลายปัจจัย</span><span class="sxs-lookup"><span data-stu-id="13edb-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="13edb-111">เปิด หรือปิดการค้นหาแฟ้มบันทึกการตรวจสอบ Office 365</span><span class="sxs-lookup"><span data-stu-id="13edb-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
