---
title: ปัญหา Microsoft Graph API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714516"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="8a08e-102">ปัญหา Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="8a08e-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="8a08e-103">หัวข้อนี้ยังอาจใช้กับนักพัฒนาที่ยังคงใช้ Azure AD Graph API</span><span class="sxs-lookup"><span data-stu-id="8a08e-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="8a08e-104">อย่างไรก็ตาม ขอแ **นะให้** คุณใช้ Microsoft Graph กับไดเรกทอรี ข้อมูลเฉพาะตัว และสถานการณ์การจัดการการเข้าถึงทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="8a08e-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="8a08e-105">**ปัญหาการรับรองความถูกต้องหรือการอนุญาต**</span><span class="sxs-lookup"><span data-stu-id="8a08e-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="8a08e-106">ถ้าแอปของคุณ **ไม่สามารถขอรับ** โทเค็นเพื่อโทรหา Microsoft Graph ได้ ให้เลือกปัญหาด้วยการรับประเภทโทเค็นการเข้าถึง (การรับรองความถูกต้อง **)** Microsoft Graph เพื่อรับความช่วยเหลือและการสนับสนุนที่เฉพาะเจาะจงมากขึ้นในหัวข้อนี้</span><span class="sxs-lookup"><span data-stu-id="8a08e-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="8a08e-107">ถ้าแอปของคุณได้รับ **ข้อผิดพลาดการอนุญาต 401 หรือ 403** เมื่อโทรหา Microsoft Graph ให้เลือกประเภทการรับการเข้าถึงที่ถูกปฏิเสธข้อผิดพลาด **(การตรวจสอบ)** API ของ Microsoft Graph เพื่อรับความช่วยเหลือและการสนับสนุนที่เฉพาะเจาะจงมากขึ้นในหัวข้อนี้</span><span class="sxs-lookup"><span data-stu-id="8a08e-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="8a08e-108">**ฉันต้องการใช้ Microsoft Graph แต่ไม่แน่ใจว่าจะเริ่มต้นที่ไหน**</span><span class="sxs-lookup"><span data-stu-id="8a08e-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="8a08e-109">ภาพรวมของ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a08e-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="8a08e-110">ภาพรวมของข้อมูลเฉพาะตัวและการจัดการการเข้าถึงใน Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a08e-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="8a08e-111">เริ่มต้นสร้างแอป Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a08e-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="8a08e-112">**Microsoft Graph Explorer** - ทดสอบ API ของ Microsoft Graph ในผู้เช่าของคุณหรือผู้เช่าการสาธิต</span><span class="sxs-lookup"><span data-stu-id="8a08e-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="8a08e-113">**ฉันต้องการใช้ Microsoft Graph แต่สนับสนุน API ไดเรกทอรี v1.0 ที่ฉันต้องการหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="8a08e-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="8a08e-114">Microsoft Graph คือ API ที่แนะนนะให้ในการจัดการไดเรกทอรี ข้อมูลเฉพาะตัว และการจัดการการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="8a08e-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="8a08e-115">อย่างไรก็ตาม ยังคงมีช่องว่างบางอย่างระหว่างสิ่งที่เป็นไปได้ใน Azure AD Graph และ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a08e-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="8a08e-116">ตรวจทานบทความต่อไปนี้ ซึ่งเน้นความแตกต่างล่าสุดเพื่อช่วยเหลือในตัวเลือกของคุณ:</span><span class="sxs-lookup"><span data-stu-id="8a08e-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="8a08e-117">ความแตกต่างของชนิดทรัพยากรระหว่าง Azure AD Graph และ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a08e-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="8a08e-118">ความแตกต่างของคุณสมบัติระหว่าง Azure AD Graph และ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a08e-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="8a08e-119">ความแตกต่างของวิธีการระหว่าง Azure AD และ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a08e-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="8a08e-120">**API ที่ฉันโทรไม่ใช้งาน - ฉันจะทดสอบเพิ่มเติมได้ที่ไหน**</span><span class="sxs-lookup"><span data-stu-id="8a08e-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="8a08e-121">**Microsoft Graph Explorer** - ทดสอบ Microsoft Graph API ในผู้เช่าของคุณหรือผู้เช่าการสาธิต และตรวจสอบคิวรี **ตัวอย่าง** ใน Microsoft Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="8a08e-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="8a08e-122">**แอปของฉันช้าเกินไปและถูกควบคุมปริมาณ ฉันสามารถปรับปรุงอะไรได้บ้าง**</span><span class="sxs-lookup"><span data-stu-id="8a08e-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="8a08e-123">ขึ้นอยู่กับสถานการณ์ของคุณ มีตัวเลือกที่หลากหลายเพื่อให้แอปพลิเคชันของคุณมีประสิทธิภาพมากขึ้น และในบางกรณี มีแนวโน้มที่จะถูกควบคุมปริมาณโดยบริการน้อยลง (เมื่อคุณโทรมากเกินไป)</span><span class="sxs-lookup"><span data-stu-id="8a08e-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="8a08e-124">หลักปฏิบัติที่ดีที่สุดของ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a08e-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="8a08e-125">การร้องขอเป็นชุด</span><span class="sxs-lookup"><span data-stu-id="8a08e-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="8a08e-126">ติดตามการเปลี่ยนแปลงผ่านคิวรีส่วนที่แตกต่าง</span><span class="sxs-lookup"><span data-stu-id="8a08e-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="8a08e-127">รับการแจ้งเตือนเกี่ยวกับการเปลี่ยนแปลงผ่าน Webhooks</span><span class="sxs-lookup"><span data-stu-id="8a08e-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="8a08e-128">แนวทางการควบคุมปริมาณ</span><span class="sxs-lookup"><span data-stu-id="8a08e-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="8a08e-129">**ฉันจะหาข้อมูลเพิ่มเติมเกี่ยวกับข้อผิดพลาดและปัญหาที่ทราบได้ที่ไหน**</span><span class="sxs-lookup"><span data-stu-id="8a08e-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="8a08e-130">ข้อมูลการตอบสนองต่อข้อผิดพลาดของ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a08e-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="8a08e-131">ปัญหาที่ทราบเกี่ยวกับ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8a08e-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="8a08e-132">**ฉันจะตรวจสอบสถานะความพร้อมของบริการและการเชื่อมต่อได้ที่ไหน**</span><span class="sxs-lookup"><span data-stu-id="8a08e-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="8a08e-133">ความพร้อมใช้งานบริการและการเชื่อมต่อของบริการที่อยู่ภายใต้การเข้าถึงผ่านทาง Microsoft Graph สามารถส่งผลกระทบต่อความพร้อมใช้งานและประสิทธิภาพโดยรวมของ Microsoft Graph ได้</span><span class="sxs-lookup"><span data-stu-id="8a08e-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="8a08e-134">สถานภาพบริการ Azure Active Directory ให้ตรวจสอบสถานะ **ของบริการความปลอดภัย +** ข้อมูลเฉพาะตัวที่แสดงใน [หน้าสถานะ Azure](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="8a08e-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="8a08e-135">บริการ Office ที่มีส่วนร่วมใน Microsoft Graph ให้ตรวจสอบสถานะของบริการที่แสดงในแดชบอร์ด[สถานภาพบริการของ Office](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="8a08e-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="8a08e-136">ข้อผิดพลาดในการตรวจสอบ Microsoft Graph อาจเป็นผลจากปัญหาต่างๆ มากมาย ซึ่งส่วนใหญ่จะสร้างข้อผิดพลาด 401 หรือ 403</span><span class="sxs-lookup"><span data-stu-id="8a08e-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="8a08e-137">ตัวอย่างเช่น สิ่งต่อไปนี้อาจก่อให้เกิดข้อผิดพลาดในการตรวจสอบได้</span><span class="sxs-lookup"><span data-stu-id="8a08e-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="8a08e-138">โฟล [ว์การรับโทเค็นการเข้าถึงที่ไม่ถูกต้อง](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="8a08e-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="8a08e-139">กําหนดขอบเขตสิทธิ์ [ได้ไม่ดี](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="8a08e-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="8a08e-140">ขาดความยินยอม[](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="8a08e-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="8a08e-141">\**_สิ้นสุดการสนับสนุนของ Azure Active Directory Authentication Library (ADAL) และ Azure AD Graph API (AAD Graph)_* _</span><span class="sxs-lookup"><span data-stu-id="8a08e-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="8a08e-142">_*เริ่มต้นวันที่ 30 มิถุนายน 2020*\* เราจะไม่เพิ่มฟีเจอร์ใหม่ใดๆ ลงใน ADAL และ Azure AD Graph อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="8a08e-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="8a08e-143">เราจะให้การสนับสนุนด้านเทคนิคและการอัปเดตความปลอดภัยต่อ แต่จะไม่มีการอัปเดตฟีเจอร์อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="8a08e-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="8a08e-144">**ตั้งแต่วันที่ 30 มิถุนายน 2022** เราจะสิ้นสุดการสนับสนุน ADAL และ Azure AD Graph และจะไม่มีการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="8a08e-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="8a08e-145">แอปที่ใช้ ADAL บนเวอร์ชัน OS ที่มีอยู่จะยังคงสามารถใช้งานต่อไปได้หลังจากนี้ *แต่จะไม่ได้รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัย* ใดๆ</span><span class="sxs-lookup"><span data-stu-id="8a08e-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="8a08e-146">แอปที่ใช้ Azure AD Graph หลังจากช่วงเวลานี้อาจไม่ได้รับการตอบกลับจากจุดสิ้นสุด Azure AD Graph อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="8a08e-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="8a08e-147">**การโยกย้าย ADAL**</span><span class="sxs-lookup"><span data-stu-id="8a08e-147">**ADAL Migration**</span></span>

<span data-ttu-id="8a08e-148">เราขอแนะนนะ [ให้อัปเดตไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)ซึ่งมีฟีเจอร์ล่าสุดและการอัปเดตความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="8a08e-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="8a08e-149">ถ้าคุณใช้งานแอปของ Microsoft ทราบว่า Microsoft อยู่ในระหว่างกระบวนการโยกย้ายแอปพลิเคชันไปยัง MSAL ภายในวันที่สิ้นสุดการสนับสนุน เพื่อให้มั่นใจว่าแอปเหล่านั้นจะได้รับประโยชน์จากการปรับปรุงความปลอดภัยและฟีเจอร์ที่ MSAL มีอย่างต่อเนื่อง</span><span class="sxs-lookup"><span data-stu-id="8a08e-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="8a08e-150">อ่าน ADAL FAQ</span><span class="sxs-lookup"><span data-stu-id="8a08e-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="8a08e-151">เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปตามแพลตฟอร์ม</span><span class="sxs-lookup"><span data-stu-id="8a08e-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="8a08e-152">ถ้าคุณต้องการความช่วยเหลือในการเข้าใจว่าแอปใดของคุณใช้ ADAL เราขอแนะนาให้คุณตรวจสอบโค้ดต้นฉบับของแอปทั้งหมด และถ้าสามารถใช้งานได้ ให้ติดต่อผู้ให้บริการ ISVs หรือแอปรายใดก็ได้</span><span class="sxs-lookup"><span data-stu-id="8a08e-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="8a08e-153">ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการของแอปที่ไม่ใช่ Microsoft ADAL ทั้งหมดในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="8a08e-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="8a08e-154">**การโยกย้ายกราฟ AAD**</span><span class="sxs-lookup"><span data-stu-id="8a08e-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="8a08e-155">สําหรับแอปพลิเคชันที่ใช้ Azure AD Graph ให้ปฏิบัติตามแนวทางของเราเพื่อ[โยกย้ายแอป Azure AD Graph ไปยัง Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="8a08e-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="8a08e-156">[รายการตรวจสอบการโยกย้ายของเราให้จุดเริ่มต้น](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)</span><span class="sxs-lookup"><span data-stu-id="8a08e-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="8a08e-157">พอร์ทัลการลงทะเบียนแอป Azure ของคุณจะแสดงแอปพลิเคชันที่ใช้ AAD Graph</span><span class="sxs-lookup"><span data-stu-id="8a08e-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="8a08e-158">เราขอแนะนนะให้คุณตรวจสอบรหัสต้นฉบับของแอปของคุณทั้งหมด และหากสามารถติดต่อผู้ให้บริการ ISVs หรือแอปใดก็ได้</span><span class="sxs-lookup"><span data-stu-id="8a08e-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="8a08e-159">ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการการใช้งาน AAD Graph ทั้งหมดในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="8a08e-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="8a08e-160">เพื่อให้แอปของคุณเข้าถึงข้อมูลใน Microsoft Graph ผู้ใช้หรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการการยินยอม</span><span class="sxs-lookup"><span data-stu-id="8a08e-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="8a08e-161">การอ้างอิง [สิทธิ์ของ Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับแต่ละชุดหลักของ Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="8a08e-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="8a08e-162">นอกจากนี้ยังมีแนวทางเกี่ยวกับวิธีการใช้สิทธิ์</span><span class="sxs-lookup"><span data-stu-id="8a08e-162">It also provides guidance about how to use the permissions.</span></span>
