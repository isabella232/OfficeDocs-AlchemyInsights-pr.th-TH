---
title: การตั้งค่า DKIM ใน Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765495"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="0c207-102">การตั้งค่า DKIM ใน Office 365</span><span class="sxs-lookup"><span data-stu-id="0c207-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="0c207-103">คำแนะนำทั้งหมดสำหรับการกำหนดค่า DKIM สำหรับโดเมนที่กำหนดเองใน Office 365 อยู่[ที่นี่](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="0c207-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="0c207-104">สำหรับ**แต่ละ**โดเมนที่กำหนดเอง คุณต้องสร้าง**สอง**ระเบียน DKIM CNAME ในโดเมนของคุณโฮสต์บริการ DNS (โดยปกติ โดเมนผู้ลงทะเบียน)</span><span class="sxs-lookup"><span data-stu-id="0c207-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="0c207-105">ตัวอย่างเช่น contoso.com และ fourthcoffee.com จำเป็นต้องมีระเบียน DKIM CNAME สี่: สำหรับ contoso.com และอีกสองเรือนสำหรับ fourthcoffee.com สองครั้ง</span><span class="sxs-lookup"><span data-stu-id="0c207-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="0c207-106">ระเบียน DKIM CNAME สำหรับ**แต่ละ**โดเมนที่กำหนดเองใช้รูปแบบต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0c207-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="0c207-107">**ชื่อโฮสต์**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="0c207-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="0c207-108">**ชี้ไปยังที่อยู่หรือค่า**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="0c207-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="0c207-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="0c207-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="0c207-110">**ชื่อโฮสต์**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="0c207-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="0c207-111">**ชี้ไปยังที่อยู่หรือค่า**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="0c207-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="0c207-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="0c207-112">**TTL**: 3600</span></span>

   <span data-ttu-id="0c207-113">\<DomainGUID\>คือข้อความที่ด้านซ้ายของ`.mail.protection.outlook.com`ในเรกคอร์ด MX แบบกำหนดเองสำหรับโดเมนกำหนดเอง (ตัวอย่างเช่น`contoso-com`สำหรับ contoso.com โดเมน)</span><span class="sxs-lookup"><span data-stu-id="0c207-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="0c207-114">\<InitialDomain\>คือโดเมนคุณใช้เมื่อคุณลงทะเบียนไว้สำหรับ Office 365 (ตัวอย่างเช่น contoso.onmicrosoft.com)</span><span class="sxs-lookup"><span data-stu-id="0c207-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="0c207-115">หลังจากที่คุณสร้างระเบียน CNAME สำหรับโดเมนของคุณเอง ทำคำแนะนำต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="0c207-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="0c207-116">อยู่</span><span class="sxs-lookup"><span data-stu-id="0c207-116">a.</span></span> <span data-ttu-id="0c207-117">[ลงชื่อเข้าใช้ Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)ด้วยบัญชีของคุณทำงาน หรือที่โรงเรียน</span><span class="sxs-lookup"><span data-stu-id="0c207-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="0c207-118">b</span><span class="sxs-lookup"><span data-stu-id="0c207-118">b.</span></span> <span data-ttu-id="0c207-119">เลือกไอคอนตัวเปิดใช้โปรแกรมประยุกต์ในด้านบนซ้าย และเลือก**Admin**</span><span class="sxs-lookup"><span data-stu-id="0c207-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="0c207-120">c</span><span class="sxs-lookup"><span data-stu-id="0c207-120">c.</span></span> <span data-ttu-id="0c207-121">ในการนำทางด้านล่างซ้าย ขยาย**Admin**และ**อัตราแลกเปลี่ยน**ที่เลือก</span><span class="sxs-lookup"><span data-stu-id="0c207-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="0c207-122">d</span><span class="sxs-lookup"><span data-stu-id="0c207-122">d.</span></span> <span data-ttu-id="0c207-123">ไปที่**การป้องกัน** > **DKIM**</span><span class="sxs-lookup"><span data-stu-id="0c207-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="0c207-124">e</span><span class="sxs-lookup"><span data-stu-id="0c207-124">e.</span></span> <span data-ttu-id="0c207-125">เลือกโดเมน และจากนั้น เลือก**เปิดใช้งาน**สำหรับ**ข้อความการเข้าสู่ระบบสำหรับโดเมนนี้มีลายเซ็น DKIM**</span><span class="sxs-lookup"><span data-stu-id="0c207-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="0c207-126">ทำซ้ำขั้นตอนนี้สำหรับแต่ละโดเมนที่กำหนดเอง</span><span class="sxs-lookup"><span data-stu-id="0c207-126">Repeat this step for each custom domain.</span></span>
