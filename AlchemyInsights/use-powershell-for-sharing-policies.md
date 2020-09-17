---
title: ใช้ PowerShell สำหรับการแชร์นโยบายและความสัมพันธ์ขององค์กร
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
ms.openlocfilehash: 378dedb332ced2c86899401c54726eb6b7e25d08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773434"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="5c1a7-102">ใช้ PowerShell สำหรับการแชร์นโยบายและความสัมพันธ์ขององค์กร</span><span class="sxs-lookup"><span data-stu-id="5c1a7-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="5c1a7-103">สำหรับความสัมพันธ์ขององค์กรโปรดตรวจทานข้อมูลไวยากรณ์และพารามิเตอร์โดยละเอียดสำหรับ: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)และการ[เอาออก OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship)</span><span class="sxs-lookup"><span data-stu-id="5c1a7-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="5c1a7-104">เมื่อต้องการสร้างนโยบายการแชร์ให้ใช้[SharingPolicy ใหม่](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy)</span><span class="sxs-lookup"><span data-stu-id="5c1a7-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="5c1a7-105">เมื่อต้องการ  [นำนโยบายการแชร์ไปใช้กับกล่องจดหมายหรือผู้ใช้](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  ที่คุณจำเป็นต้องใช้การรวมกันของ  [กล่องจดหมายตั้งค่า](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) และ [กล่องจดหมายเข้า](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) ที่มีนโยบายที่สร้างขึ้นใหม่</span><span class="sxs-lookup"><span data-stu-id="5c1a7-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="5c1a7-106">เมื่อต้องการ[ปรับเปลี่ยนปิดใช้งานหรือเอานโยบายการแชร์](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)ที่คุณจำเป็นต้องใช้ในการ[ตั้งค่า SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy)และ[เอาออก SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)</span><span class="sxs-lookup"><span data-stu-id="5c1a7-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="5c1a7-107">**สำหรับการทำความเข้าใจเกี่ยวกับหัวข้อนี้อย่างสมบูรณ์โปรดอ่าน:**</span><span class="sxs-lookup"><span data-stu-id="5c1a7-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="5c1a7-108">การแชร์ใน Exchange Online</span><span class="sxs-lookup"><span data-stu-id="5c1a7-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)