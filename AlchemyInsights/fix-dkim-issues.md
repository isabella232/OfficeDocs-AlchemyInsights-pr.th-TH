---
title: แก้ไขปัญหาการตั้งค่าของ DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765483"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="60212-102">แก้ไขปัญหาการตั้งค่าของ DKIM</span><span class="sxs-lookup"><span data-stu-id="60212-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="60212-103">ถ้าคุณประสบปัญหาในการเปิดใช้งาน DKIM สำหรับโดเมนของคุณเอง ให้ใช้ขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="60212-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="60212-104">ปัญหาการตั้งค่า DKIM ส่วนใหญ่เกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="60212-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="60212-105">ตรวจสอบระเบียน DKIM CNAME (**ไม่**เรกคอร์ด TXT) ถูกจัดรูปแบบอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="60212-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="60212-106">สำหรับข้อมูลเพิ่มเติม ให้ดู[หัวข้อ](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)นี้</span><span class="sxs-lookup"><span data-stu-id="60212-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="60212-107">หลังจากที่คุณสร้าง หรือปรับปรุงระเบียน DKIM DNS ของคุณใน DNS โฮสต์การบริการสำหรับโดเมนของคุณ (โดยทั่วไป ของโดเมนผู้ลงทะเบียน) รอสำหรับระเบียน DNS ที่จะเผยแพร่</span><span class="sxs-lookup"><span data-stu-id="60212-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="60212-108">ถ้าคุณไม่สามารถสร้าง DKIM DNS ระเบียนใน admin ศูนย์ คุณสามารถแทน\<CustomDomain\>กับโดเมนของคุณเอง (ตัวอย่างเช่น contoso.com) และเรียกใช้คำสั่งนี้ใน[PowerShell ออนไลน์ของ Exchange](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):`New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`ได้</span><span class="sxs-lookup"><span data-stu-id="60212-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
