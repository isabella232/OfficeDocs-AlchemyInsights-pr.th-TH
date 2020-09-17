---
title: ตั้งค่า DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808726"
---
# <a name="setup-dkim"></a><span data-ttu-id="a6d47-102">ตั้งค่า DKIM</span><span class="sxs-lookup"><span data-stu-id="a6d47-102">Setup DKIM</span></span>

<span data-ttu-id="a6d47-103">คำแนะนำที่สมบูรณ์สำหรับการกำหนดค่า DKIM สำหรับโดเมนแบบกำหนดเองใน Microsoft ๓๖๕อยู่[ที่นี่](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)</span><span class="sxs-lookup"><span data-stu-id="a6d47-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="a6d47-104">สำหรับ **แต่ละ** โดเมนแบบกำหนดเองคุณจะต้องสร้างระเบียน CNAME ของ DKIM **สอง** ระเบียนที่บริการโฮสต์ DNS ของโดเมนของคุณ (โดยทั่วไปคือบริษัทจดทะเบียนโดเมน)</span><span class="sxs-lookup"><span data-stu-id="a6d47-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="a6d47-105">ตัวอย่างเช่น contoso.com และ fourthcoffee.com จำเป็นต้องมีระเบียน CNAME ของ DKIM สี่ระเบียน: สองสำหรับ contoso.com และสองสำหรับ fourthcoffee.com</span><span class="sxs-lookup"><span data-stu-id="a6d47-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="a6d47-106">ระเบียน CNAME ของ DKIM สำหรับ **แต่ละ** โดเมนแบบกำหนดเองจะใช้รูปแบบต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a6d47-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="a6d47-107">**ชื่อโฮสต์**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="a6d47-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="a6d47-108">**ชี้ไปยังที่อยู่หรือค่า**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="a6d47-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="a6d47-109">**TTL**: ๓๖๐๐</span><span class="sxs-lookup"><span data-stu-id="a6d47-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="a6d47-110">**ชื่อโฮสต์**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="a6d47-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="a6d47-111">**ชี้ไปยังที่อยู่หรือค่า**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="a6d47-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="a6d47-112">**TTL**: ๓๖๐๐</span><span class="sxs-lookup"><span data-stu-id="a6d47-112">**TTL**: 3600</span></span>

   <span data-ttu-id="a6d47-113">\<DomainGUID\> เป็นข้อความทางด้านซ้ายของ `.mail.protection.outlook.com` ระเบียน MX ที่กำหนดเองสำหรับโดเมนแบบกำหนดเอง (ตัวอย่างเช่น `contoso-com` สำหรับโดเมน contoso.com)</span><span class="sxs-lookup"><span data-stu-id="a6d47-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="a6d47-114">\<InitialDomain\> โดเมนที่คุณใช้เมื่อคุณลงชื่อเข้าใช้ Microsoft ๓๖๕ (ตัวอย่างเช่น contoso.onmicrosoft.com)</span><span class="sxs-lookup"><span data-stu-id="a6d47-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="a6d47-115">หลังจากที่คุณได้สร้างระเบียน CNAME สำหรับโดเมนแบบกำหนดเองของคุณแล้วให้ทำตามคำแนะนำต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="a6d47-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="a6d47-116">a.</span><span class="sxs-lookup"><span data-stu-id="a6d47-116">a.</span></span> <span data-ttu-id="a6d47-117">[ลงชื่อเข้าใช้ Microsoft ๓๖๕](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) ด้วยบัญชีผู้ใช้ของที่ทำงานหรือที่โรงเรียนของคุณ</span><span class="sxs-lookup"><span data-stu-id="a6d47-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="a6d47-118">b.</span><span class="sxs-lookup"><span data-stu-id="a6d47-118">b.</span></span> <span data-ttu-id="a6d47-119">เลือกไอคอนตัวเปิดใช้งานแอปที่มุมบนซ้ายแล้วเลือก**ผู้ดูแลระบบ**</span><span class="sxs-lookup"><span data-stu-id="a6d47-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="a6d47-120">c.</span><span class="sxs-lookup"><span data-stu-id="a6d47-120">c.</span></span> <span data-ttu-id="a6d47-121">ในการนำทางด้านซ้ายล่างให้ขยาย**ผู้ดูแลระบบ**แล้วเลือก**Exchange**</span><span class="sxs-lookup"><span data-stu-id="a6d47-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="a6d47-122">d.</span><span class="sxs-lookup"><span data-stu-id="a6d47-122">d.</span></span> <span data-ttu-id="a6d47-123">ไปที่การ**ป้องกัน**  >  **DKIM**</span><span class="sxs-lookup"><span data-stu-id="a6d47-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="a6d47-124">e.</span><span class="sxs-lookup"><span data-stu-id="a6d47-124">e.</span></span> <span data-ttu-id="a6d47-125">เลือกโดเมนแล้วเลือก**เปิดใช้งาน**สำหรับการ**เซ็นชื่อข้อความสำหรับโดเมนนี้กับลายเซ็น DKIM**</span><span class="sxs-lookup"><span data-stu-id="a6d47-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="a6d47-126">ทำซ้ำขั้นตอนนี้สำหรับแต่ละโดเมนแบบกำหนดเอง</span><span class="sxs-lookup"><span data-stu-id="a6d47-126">Repeat this step for each custom domain.</span></span>
