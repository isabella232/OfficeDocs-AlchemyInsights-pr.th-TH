---
title: แก้ไขปัญหาการตั้งค่า DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506793"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="13728-102">แก้ไขปัญหาการตั้งค่า DKIM</span><span class="sxs-lookup"><span data-stu-id="13728-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="13728-103">หากคุณพบปัญหาในการเปิดใช้งาน DKIM สําหรับโดเมนแบบกําหนดเอง ของคุณ ให้ใช้ขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="13728-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="13728-104">ปัญหาการตั้งค่า DKIM ส่วนใหญ่เกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="13728-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="13728-105">ตรวจสอบระเบียน CNAME DKIM (**ไม่ใช่**ระเบียน TXT) ถูกจัดรูปแบบอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="13728-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="13728-106">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)</span><span class="sxs-lookup"><span data-stu-id="13728-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="13728-107">หลังจากที่คุณสร้างหรืออัปเดตระเบียน DNS DKIM ของคุณที่บริการโฮสต์ DNS สําหรับโดเมนของคุณ (โดยทั่วไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="13728-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="13728-108">ถ้าคุณไม่สามารถสร้างระเบียน DNS DKIM ใน \<CustomDomain\> contoso.com[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)ศูนย์การจัดการ `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`</span><span class="sxs-lookup"><span data-stu-id="13728-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
