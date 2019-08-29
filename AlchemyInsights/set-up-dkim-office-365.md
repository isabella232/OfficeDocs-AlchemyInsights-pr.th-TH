---
title: ตั้งค่า DKIM ใน Office ๓๖๕
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666283"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="44b0a-102">ตั้งค่า DKIM ใน Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="44b0a-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="44b0a-103">คำแนะนำที่สมบูรณ์สำหรับการกำหนดค่า DKIM สำหรับโดเมนที่กำหนดเองใน Office ๓๖๕อยู่ที่[นี่](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="44b0a-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="44b0a-104">สำหรับ**แต่ละ**โดเมนที่กำหนดเองคุณจำเป็นต้องสร้างระเบียน CNAME แบบ DKIM **2**รายการที่บริการโฮสต์ DNS ของโดเมนของคุณ (โดยทั่วไปคือผู้ลงทะเบียนโดเมน)</span><span class="sxs-lookup"><span data-stu-id="44b0a-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="44b0a-105">ตัวอย่างเช่น contoso.com และ fourthcoffee.com ต้องการระเบียน DKIM CNAME สี่เรกคอร์ด: สองสำหรับ contoso.com และสองสำหรับ fourthcoffee.com</span><span class="sxs-lookup"><span data-stu-id="44b0a-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="44b0a-106">ระเบียน DKIM CNAME สำหรับ**แต่ละ**โดเมนที่กำหนดเองจะใช้รูปแบบต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="44b0a-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="44b0a-107">**ชื่อโฮสต์**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="44b0a-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="44b0a-108">**ชี้ไปที่ที่อยู่หรือค่า**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="44b0a-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="44b0a-109">**TTL**: ๓๖๐๐</span><span class="sxs-lookup"><span data-stu-id="44b0a-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="44b0a-110">**ชื่อโฮสต์**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="44b0a-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="44b0a-111">**ชี้ไปที่ที่อยู่หรือค่า**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="44b0a-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="44b0a-112">**TTL**: ๓๖๐๐</span><span class="sxs-lookup"><span data-stu-id="44b0a-112">**TTL**: 3600</span></span>

   <span data-ttu-id="44b0a-113">\<DomainGUID\>คือข้อความทางด้านซ้ายของ`.mail.protection.outlook.com`ระเบียน MX ที่กำหนดเองสำหรับโดเมนที่กำหนดเอง (ตัว`contoso-com`อย่างเช่นสำหรับโดเมน contoso.com)</span><span class="sxs-lookup"><span data-stu-id="44b0a-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="44b0a-114">\<ต้นแบบโด\>เมนคือโดเมนที่คุณใช้เมื่อคุณลงทะเบียนสำหรับ Office ๓๖๕ (ตัวอย่างเช่น contoso.onmicrosoft.com)</span><span class="sxs-lookup"><span data-stu-id="44b0a-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="44b0a-115">หลังจากที่คุณได้สร้างระเบียน CNAME สำหรับโดเมนที่กำหนดเองของคุณแล้วให้ทำตามคำแนะนำต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="44b0a-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="44b0a-116">ราคา .</span><span class="sxs-lookup"><span data-stu-id="44b0a-116">a.</span></span> <span data-ttu-id="44b0a-117">[ลงชื่อเข้าใช้ Office ๓๖๕](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)ด้วยบัญชีที่ทำงานหรือที่โรงเรียนของคุณ</span><span class="sxs-lookup"><span data-stu-id="44b0a-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="44b0a-118">B</span><span class="sxs-lookup"><span data-stu-id="44b0a-118">b.</span></span> <span data-ttu-id="44b0a-119">เลือกไอคอนตัวเปิดแอพในด้านบนซ้ายและเลือกผู้**ดูแล**</span><span class="sxs-lookup"><span data-stu-id="44b0a-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="44b0a-120">C</span><span class="sxs-lookup"><span data-stu-id="44b0a-120">c.</span></span> <span data-ttu-id="44b0a-121">ในการนำทางด้านซ้ายล่างให้ขยายผู้**ดูแล**และเลือก**แลกเปลี่ยน**</span><span class="sxs-lookup"><span data-stu-id="44b0a-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="44b0a-122">D</span><span class="sxs-lookup"><span data-stu-id="44b0a-122">d.</span></span> <span data-ttu-id="44b0a-123">ไปที่**DKIM**ของ**การป้องกัน** > </span><span class="sxs-lookup"><span data-stu-id="44b0a-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="44b0a-124">ตะวัน ออก</span><span class="sxs-lookup"><span data-stu-id="44b0a-124">e.</span></span> <span data-ttu-id="44b0a-125">เลือกโดเมนแล้วเลือก**เปิดใช้งาน**สำหรับ**ข้อความลงชื่อสำหรับโดเมนนี้ด้วยลายเซ็น DKIM**</span><span class="sxs-lookup"><span data-stu-id="44b0a-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="44b0a-126">ทำซ้ำขั้นตอนนี้สำหรับแต่ละโดเมนที่กำหนดเอง</span><span class="sxs-lookup"><span data-stu-id="44b0a-126">Repeat this step for each custom domain.</span></span>
