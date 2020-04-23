---
title: แก้ไขปัญหาการติดตั้ง DKIM
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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717581"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="1623f-102">แก้ไขปัญหาการติดตั้ง DKIM</span><span class="sxs-lookup"><span data-stu-id="1623f-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="1623f-103">หากคุณประสบปัญหาในการเปิดใช้ DKIM สําหรับโดเมนแบบกําหนดเอง ให้ทําตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="1623f-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="1623f-104">ปัญหาการตั้งค่า DKIM ส่วนใหญ่เกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="1623f-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="1623f-105">ตรวจสอบว่าระเบียน CNAME DKIM (**ไม่ใช่**ระเบียน TXT) ถูกจัดรูปแบบอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="1623f-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="1623f-106">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[หัวข้อนี้](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="1623f-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="1623f-107">หลังจากที่คุณสร้างหรืออัปเดตระเบียน DNS DKIM ที่บริการโฮสต์ DNS สําหรับโดเมนของคุณ (โดยทั่วไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="1623f-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="1623f-108">ถ้าคุณไม่สามารถสร้างระเบียน DNS DKIM ใน\<contoso.com\>[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)`New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`ศูนย์การจัดการ</span><span class="sxs-lookup"><span data-stu-id="1623f-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
