---
title: การตั้งค่า DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509403"
---
# <a name="setup-dkim"></a><span data-ttu-id="9ebfc-102">การตั้งค่า DKIM</span><span class="sxs-lookup"><span data-stu-id="9ebfc-102">Setup DKIM</span></span>

<span data-ttu-id="9ebfc-103">คําแนะนําฉบับสมบูรณ์สําหรับการกําหนดค่า DKIM สําหรับโดเมนแบบกําหนดเองใน Microsoft 365[อยู่ที่นี่](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)</span><span class="sxs-lookup"><span data-stu-id="9ebfc-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="9ebfc-104">สําหรับโดเมนที่กําหนดเอง**แต่ละ**โดเมน คุณจะต้องสร้างระเบียน DKIM CNAME**สอง**รายการที่บริการโฮสต์ DNS ของโดเมน (โดยทั่วไปแล้ว</span><span class="sxs-lookup"><span data-stu-id="9ebfc-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="9ebfc-105">ตัวอย่างเช่น contoso.com และfourthcoffee.comต้องการระเบียน DKIM CNAME สี่รายการ ได้แก่ สองสําหรับcontoso.comและสองสําหรับfourthcoffee.com</span><span class="sxs-lookup"><span data-stu-id="9ebfc-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="9ebfc-106">ระเบียน CNAME DKIM**สําหรับแต่ละโดเมน**แบบกําหนดเองใช้รูปแบบต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="9ebfc-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="9ebfc-107">**ชื่อโฮสต์**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="9ebfc-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="9ebfc-108">**ที่อยู่หรือค่าชี้ถึง**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="9ebfc-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="9ebfc-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="9ebfc-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="9ebfc-110">**ชื่อโฮสต์**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="9ebfc-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="9ebfc-111">**ที่อยู่หรือค่าชี้ถึง**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="9ebfc-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="9ebfc-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="9ebfc-112">**TTL**: 3600</span></span>

   <span data-ttu-id="9ebfc-113">\<DomainGUID\>ข้อความทางด้านซ้ายของระเบียน MX `.mail.protection.outlook.com` ที่กําหนดเองสําหรับโดเมนแบบกําหนดเอง (ตัวอย่างเช่น `contoso-com` สําหรับโดเมนcontoso.com)</span><span class="sxs-lookup"><span data-stu-id="9ebfc-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="9ebfc-114">\<InitialDomain\>คือโดเมนที่คุณใช้เมื่อคุณลงทะเบียนสําหรับ Microsoft 365 (ตัวอย่างเช่น contoso.onmicrosoft.com)</span><span class="sxs-lookup"><span data-stu-id="9ebfc-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="9ebfc-115">หลังจากที่คุณสร้างระเบียน CNAME สําหรับโดเมนแบบกําหนดเองแล้ว ให้ทําตามคําแนะนําต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="9ebfc-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="9ebfc-116">a.</span><span class="sxs-lookup"><span data-stu-id="9ebfc-116">a.</span></span> <span data-ttu-id="9ebfc-117">[ลงชื่อเข้าใช้ Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4)ด้วยบัญชีที่ทํางานหรือโรงเรียนของคุณ</span><span class="sxs-lookup"><span data-stu-id="9ebfc-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="9ebfc-118">b.</span><span class="sxs-lookup"><span data-stu-id="9ebfc-118">b.</span></span> <span data-ttu-id="9ebfc-119">เลือกไอคอนตัวเปิดใช้แอปที่ด้านซ้ายบน แล้วเลือก**ผู้ดูแลระบบ**</span><span class="sxs-lookup"><span data-stu-id="9ebfc-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="9ebfc-120">c.</span><span class="sxs-lookup"><span data-stu-id="9ebfc-120">c.</span></span> <span data-ttu-id="9ebfc-121">ในการนําทางด้านซ้ายล่าง ให้ขยาย**ผู้ดูแลระบบ**แล้วเลือก**Exchange**</span><span class="sxs-lookup"><span data-stu-id="9ebfc-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="9ebfc-122">D</span><span class="sxs-lookup"><span data-stu-id="9ebfc-122">d.</span></span> <span data-ttu-id="9ebfc-123">ไปที่**Protection**  >  **DKIM**การป้องกัน</span><span class="sxs-lookup"><span data-stu-id="9ebfc-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="9ebfc-124">ตะวัน ออก</span><span class="sxs-lookup"><span data-stu-id="9ebfc-124">e.</span></span> <span data-ttu-id="9ebfc-125">เลือกโดเมน แล้วเลือก**เปิดใช้งาน**สําหรับ**ข้อความลงชื่อ สําหรับโดเมนนี้ด้วยลายเซ็น DKIM**</span><span class="sxs-lookup"><span data-stu-id="9ebfc-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="9ebfc-126">ทําซ้ําขั้นตอนนี้สําหรับแต่ละโดเมนแบบกําหนดเอง</span><span class="sxs-lookup"><span data-stu-id="9ebfc-126">Repeat this step for each custom domain.</span></span>
