---
title: แก้ไขปัญหาทั่วไปเกี่ยวกับการจัดรูปแบบระเบียน DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525643"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="6316b-102">แก้ไขปัญหาทั่วไปเกี่ยวกับการจัดรูปแบบระเบียน DKIM</span><span class="sxs-lookup"><span data-stu-id="6316b-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="6316b-103">ปัญหาการตั้งค่า DKIM ส่วนใหญ่เกี่ยวข้องกับระเบียน DNS ที่ไม่ถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="6316b-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="6316b-104">เมื่อต้องการแก้ไขปัญหาการตั้งค่า DKIM ให้ตรวจสอบว่าระเบียน CNAME ของ DKIM **(ไม่ใช่** ระเบียน TXT) ได้รับการจัดรูปแบบอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="6316b-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="6316b-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="6316b-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="6316b-106">ถ้าคุณต้องการความช่วยเหลือเกี่ยวกับระเบียน DNS โดยทั่วไป ให้ดูที่ สร้างระเบียน[DNS ที่ผู้ให้บริการโฮสต์ DNS ใดก็ได้ของ Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)</span><span class="sxs-lookup"><span data-stu-id="6316b-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="6316b-107">หลังจากที่คุณสร้างหรืออัปเดตระเบียน DNS DKIM ของคุณที่บริการโฮสต์ DNS ให้กับโดเมนของคุณแล้ว คุณจะต้องรอให้ระเบียน DNS เผยแพร่</span><span class="sxs-lookup"><span data-stu-id="6316b-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
