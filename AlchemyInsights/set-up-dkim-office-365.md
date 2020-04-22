---
title: ติดตั้ง DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645691"
---
# <a name="setup-dkim"></a><span data-ttu-id="cd7ce-102">ติดตั้ง DKIM</span><span class="sxs-lookup"><span data-stu-id="cd7ce-102">Setup DKIM</span></span>

<span data-ttu-id="cd7ce-103">คําแนะนําที่สมบูรณ์สําหรับการกําหนดค่า DKIM สําหรับโดเมนแบบกําหนดเองใน Microsoft 365[อยู่ที่นี่](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="cd7ce-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="cd7ce-104">สําหรับโดเมนที่กําหนดเอง**แต่ละ**โดเมน คุณจะต้องสร้างระเบียน DKIM CNAME**สอง**ระเบียนที่บริการโฮสต์ DNS ของโดเมน (โดยทั่วไปคือ บริษัทจดทะเบียนโดเมน)</span><span class="sxs-lookup"><span data-stu-id="cd7ce-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="cd7ce-105">ตัวอย่างเช่น contoso.comและfourthcoffee.comต้องใช้ระเบียน DKIM CNAME 4 ระเบียน คือ สองระเบียนสําหรับcontoso.comและสองระเบียนสําหรับfourthcoffee.com</span><span class="sxs-lookup"><span data-stu-id="cd7ce-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="cd7ce-106">ระเบียน CNAME ของ DKIM**สําหรับแต่ละโดเมน**ที่กําหนดเองใช้รูปแบบต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="cd7ce-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="cd7ce-107">**ชื่อโฮสต์**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="cd7ce-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="cd7ce-108">**ที่อยู่หรือค่า**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="cd7ce-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="cd7ce-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="cd7ce-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="cd7ce-110">**ชื่อโฮสต์**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="cd7ce-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="cd7ce-111">**ที่อยู่หรือค่า**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="cd7ce-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="cd7ce-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="cd7ce-112">**TTL**: 3600</span></span>

   <span data-ttu-id="cd7ce-113">\<DomainGUID\>คือข้อความทางด้านซ้ายของ`.mail.protection.outlook.com`ระเบียน MX ที่กําหนดเองสําหรับโดเมนแบบกําหนดเอง (ตัวอย่างเช่น`contoso-com`สําหรับโดเมนcontoso.com)</span><span class="sxs-lookup"><span data-stu-id="cd7ce-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="cd7ce-114">\<InitialDomain\>คือโดเมนที่คุณใช้เมื่อคุณลงทะเบียนสําหรับ Microsoft 365 (ตัวอย่างเช่น contoso.onmicrosoft.com)</span><span class="sxs-lookup"><span data-stu-id="cd7ce-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="cd7ce-115">หลังจากที่คุณได้สร้างระเบียน CNAME สําหรับโดเมนแบบกําหนดเองของคุณแล้ว ให้ปฏิบัติตามคําแนะนําต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="cd7ce-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="cd7ce-116">ก.ส.</span><span class="sxs-lookup"><span data-stu-id="cd7ce-116">a.</span></span> <span data-ttu-id="cd7ce-117">[ลงชื่อเข้าใช้ Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)ด้วยบัญชีที่ทํางานหรือที่โรงเรียนของคุณ</span><span class="sxs-lookup"><span data-stu-id="cd7ce-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="cd7ce-118">B</span><span class="sxs-lookup"><span data-stu-id="cd7ce-118">b.</span></span> <span data-ttu-id="cd7ce-119">เลือกไอคอนตัวเปิดใช้แอปที่ด้านบนซ้าย แล้วเลือก**ผู้ดูแลระบบ**</span><span class="sxs-lookup"><span data-stu-id="cd7ce-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="cd7ce-120">C</span><span class="sxs-lookup"><span data-stu-id="cd7ce-120">c.</span></span> <span data-ttu-id="cd7ce-121">ในการนําทางด้านซ้ายล่าง ให้ขยาย**ผู้ดูแลระบบ**แล้วเลือก**Exchange**</span><span class="sxs-lookup"><span data-stu-id="cd7ce-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="cd7ce-122">D</span><span class="sxs-lookup"><span data-stu-id="cd7ce-122">d.</span></span> <span data-ttu-id="cd7ce-123">ไปที่**การป้องกัน** > **DKIM**</span><span class="sxs-lookup"><span data-stu-id="cd7ce-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="cd7ce-124">ตะวัน ออก</span><span class="sxs-lookup"><span data-stu-id="cd7ce-124">e.</span></span> <span data-ttu-id="cd7ce-125">เลือกโดเมน แล้วเลือก**เปิดใช้งาน**สําหรับ**เซ็นชื่อข้อความสําหรับโดเมนนี้ด้วยลายเซ็น DKIM**</span><span class="sxs-lookup"><span data-stu-id="cd7ce-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="cd7ce-126">ทําซ้ําขั้นตอนนี้สําหรับแต่ละโดเมนแบบกําหนดเอง</span><span class="sxs-lookup"><span data-stu-id="cd7ce-126">Repeat this step for each custom domain.</span></span>
