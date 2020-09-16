---
title: แก้ไขปัญหาการตั้งค่า DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744969"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="41af0-102">แก้ไขปัญหาการตั้งค่า DKIM</span><span class="sxs-lookup"><span data-stu-id="41af0-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="41af0-103">ถ้าคุณประสบปัญหาในการเปิดใช้งาน DKIM สำหรับโดเมนแบบกำหนดเองของคุณให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="41af0-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="41af0-104">ปัญหาการตั้งค่า DKIM ส่วนใหญ่จะเกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="41af0-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="41af0-105">ตรวจสอบระเบียน CNAME ของ DKIM (**ไม่ใช่** ระเบียน TXT) ถูกจัดรูปแบบอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="41af0-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="41af0-106">สำหรับข้อมูลเพิ่มเติมให้ดู [หัวข้อ](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)นี้</span><span class="sxs-lookup"><span data-stu-id="41af0-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="41af0-107">หลังจากที่คุณสร้างหรืออัปเดตระเบียน DNS DKIM ของคุณที่บริการโฮสต์ DNS สำหรับโดเมนของคุณ (โดยทั่วไปแล้วบริษัทจดทะเบียนโดเมนของคุณ) ให้รอระเบียน DNS เพื่อเผยแพร่</span><span class="sxs-lookup"><span data-stu-id="41af0-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="41af0-108">ถ้าคุณไม่สามารถสร้างเรกคอร์ด DNS DKIM ในศูนย์การจัดการได้คุณสามารถแทน \<CustomDomain\> ที่ด้วยโดเมนแบบกำหนดเองของคุณ (ตัวอย่างเช่น contoso.com) และเรียกใช้คำสั่งนี้ใน[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`</span><span class="sxs-lookup"><span data-stu-id="41af0-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
