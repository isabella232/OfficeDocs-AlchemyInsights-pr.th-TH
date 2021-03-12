---
title: ใช้ PowerShell เพื่อแชร์นโยบายและความสัมพันธ์ขององค์กร
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
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709485"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>ใช้ PowerShell เพื่อแชร์นโยบายและความสัมพันธ์ขององค์กร


For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation,](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation) [New-OrganizationRelationship,](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship) [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). เมื่อต้องการ  [ใช้นโยบายการแชร์กับกล่องจดหมายหรือ](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  ผู้ใช้ คุณจึงต้องใช้การผสมผสานของ  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) และ [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) กับนโยบายที่สร้างขึ้นใหม่ To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**เพื่อความเข้าใจแบบเต็มเกี่ยวกับหัวข้อนี้ โปรดอ่าน:**

[การแชร์ใน Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)