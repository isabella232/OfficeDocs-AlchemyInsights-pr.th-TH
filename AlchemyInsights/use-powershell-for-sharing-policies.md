---
title: ใช้ PowerShell สําหรับนโยบายและความสัมพันธ์ขององค์กรร่วมกัน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862158"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="5d1fe-102">ใช้ PowerShell สําหรับนโยบายและความสัมพันธ์ขององค์กรร่วมกัน</span><span class="sxs-lookup"><span data-stu-id="5d1fe-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="5d1fe-103">สําหรับความสัมพันธ์ขององค์กรโปรดตรวจทานไวยากรณ์และพารามิเตอร์รายละเอียดสําหรับ :[รับสหพันธรัฐ ,](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation)[องค์กรใหม่Relationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set - OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)และลบ - [OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="5d1fe-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="5d1fe-104">เมื่อต้องการสร้างนโยบายการแชร์ให้ใช้['ร่วมกันใหม่'](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)</span><span class="sxs-lookup"><span data-stu-id="5d1fe-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="5d1fe-105">เมื่อต้องการ[ใช้นโยบายการใช้ร่วมกันกับกล่องจดหมายหรือผู้ใช้](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)คุณจําเป็นต้องใช้ชุด[กล่องจดหมาย](https://docs.microsoft.com/powershell/module/exchange/set-mailbox)และ[กล่องจดหมายรับ](https://docs.microsoft.com/powershell/module/exchange/get-mailbox)กับนโยบายที่สร้างขึ้นใหม่</span><span class="sxs-lookup"><span data-stu-id="5d1fe-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="5d1fe-106">เมื่อต้องการ[ปรับเปลี่ยน ปิดใช้งาน หรือเอานโยบายการใช้ร่วมกัน](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)ออก คุณต้องใช้[การตั้งค่าร่วมกันPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy)และ[เอาใช้งานร่วมกันPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)</span><span class="sxs-lookup"><span data-stu-id="5d1fe-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="5d1fe-107">**สําหรับความเข้าใจเต็มรูปแบบของหัวข้อนี้โปรดอ่าน :**</span><span class="sxs-lookup"><span data-stu-id="5d1fe-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="5d1fe-108">การใช้ร่วมกันในการแลกเปลี่ยนแบบออนไลน์</span><span class="sxs-lookup"><span data-stu-id="5d1fe-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)