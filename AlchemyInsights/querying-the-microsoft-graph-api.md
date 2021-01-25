---
title: การสอบถาม API ของ Microsoft Graph
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974688"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="75608-102">การสอบถาม API ของ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="75608-103">หัวข้อนี้ยังอาจนำไปใช้กับนักพัฒนายังคงใช้ Azure AD Graph API</span><span class="sxs-lookup"><span data-stu-id="75608-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="75608-104">อย่างไรก็ตาม **ขอแนะนำให้คุณ** ใช้ Microsoft Graph สำหรับสถานการณ์สมมติของไดเรกทอรีข้อมูลประจำตัวและการจัดการการเข้าถึงทั้งหมดของคุณ</span><span class="sxs-lookup"><span data-stu-id="75608-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="75608-105">**ปัญหาเกี่ยวกับการรับรองความถูกต้องหรือการอนุญาต**</span><span class="sxs-lookup"><span data-stu-id="75608-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="75608-106">ถ้าแอปของคุณไม่ **สามารถรับโทเค็น** การโทรถึง microsoft graph ได้ให้เลือก **ปัญหาเกี่ยวกับการรับโทเค็นการเข้าถึง (การรับรองความถูกต้อง)** ประเภท Microsoft Graph เพื่อรับความช่วยเหลือและการสนับสนุนที่เฉพาะเจาะจงมากขึ้นในหัวข้อนี้</span><span class="sxs-lookup"><span data-stu-id="75608-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="75608-107">ถ้าแอปของคุณได้ **รับข้อผิดพลาด** ในการอนุญาตให้ใช้งาน๔๐๑หรือ๔๐๓เมื่อโทรหา microsoft graph ให้เลือกประเภทการ **รับข้อผิดพลาดในการปฏิเสธการเข้าถึง (การอนุญาต)** Microsoft Graph API เพื่อรับความช่วยเหลือและการสนับสนุนที่เฉพาะเจาะจงมากขึ้นในหัวข้อนี้</span><span class="sxs-lookup"><span data-stu-id="75608-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="75608-108">**ฉันต้องการใช้ Microsoft Graph แต่ไม่แน่ใจว่าจะเริ่มต้นที่ใด**</span><span class="sxs-lookup"><span data-stu-id="75608-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="75608-109">เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับ Microsoft Graph ให้ดู:</span><span class="sxs-lookup"><span data-stu-id="75608-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="75608-110">ภาพรวมของ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="75608-111">ภาพรวมของการจัดการข้อมูลประจำตัวและการเข้าถึงใน Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="75608-112">การเริ่มต้นใช้งานแอป Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="75608-113">**Microsoft Graph Explorer** -ทดสอบ Microsoft graph APIs ในผู้เช่าของคุณหรือผู้เช่าสาธิต</span><span class="sxs-lookup"><span data-stu-id="75608-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="75608-114">**ฉันต้องการใช้ Microsoft Graph แต่สนับสนุนไดเรกทอรี v1.0 ที่ฉันจำเป็นต้องใช้**</span><span class="sxs-lookup"><span data-stu-id="75608-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="75608-115">Microsoft Graph เป็น API ที่แนะนำสำหรับไดเรกทอรีข้อมูลประจำตัวและการจัดการการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="75608-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="75608-116">อย่างไรก็ตามยังมีช่องว่างไม่กี่ช่องระหว่างสิ่งที่เป็นไปได้ในกราฟโฆษณา Azure และ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="75608-117">ตรวจทานบทความต่อไปนี้ซึ่งเน้นความแตกต่างล่าสุดสำหรับความช่วยเหลือในตัวเลือกของคุณ:</span><span class="sxs-lookup"><span data-stu-id="75608-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="75608-118">ความแตกต่างของชนิดทรัพยากรระหว่างกราฟ AD Azure และ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="75608-119">ความแตกต่างของคุณสมบัติระหว่างกราฟโฆษณา Azure และ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="75608-120">ความแตกต่างของวิธีการระหว่าง Azure AD และ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="75608-121">**เมื่อฉันสอบถามวัตถุ *ผู้ใช้* หลายคุณสมบัติจะหายไป**</span><span class="sxs-lookup"><span data-stu-id="75608-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="75608-122">`GET https://graph.microsoft.com/v1.0/users` ส่งกลับเฉพาะที่พัก11แห่งเนื่องจาก Microsoft Graph จะเลือกชุดของคุณสมบัติของ *ผู้ใช้* ที่จะส่งกลับเป็นค่าเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="75608-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="75608-123">ถ้าคุณต้องการคุณสมบัติของ *ผู้ใช้* อื่นให้ใช้ $select เพื่อเลือกคุณสมบัติของแอปพลิเคชันที่คุณต้องการ</span><span class="sxs-lookup"><span data-stu-id="75608-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="75608-124">ลองใช้งานใน **Microsoft Graph Explorer** ก่อน</span><span class="sxs-lookup"><span data-stu-id="75608-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="75608-125">**ค่าคุณสมบัติของผู้ใช้บางค่าเป็น *null* แม้ว่าฉันจะได้รับการตั้งค่า**</span><span class="sxs-lookup"><span data-stu-id="75608-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="75608-126">คำอธิบายที่เป็นไปได้มากที่สุดคือแอปพลิเคชันที่ได้รับอนุญาตให้ *ผู้ใช้ ReadBasic*</span><span class="sxs-lookup"><span data-stu-id="75608-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="75608-127">การดำเนินการนี้จะช่วยให้แอปพลิเคชันอ่านคุณสมบัติของผู้ใช้ที่จำกัดและส่งกลับค่าคุณสมบัติอื่นๆทั้งหมดเป็น null แม้ว่าจะได้รับการตั้งค่าก่อนหน้านี้แล้ว</span><span class="sxs-lookup"><span data-stu-id="75608-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="75608-128">ลองให้สิทธิ์ผู้ใช้แอปพลิเคชัน *อ่านสิทธิ์ทั้งหมด* แทน</span><span class="sxs-lookup"><span data-stu-id="75608-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="75608-129">สำหรับข้อมูลเพิ่มเติมให้ดูที่[สิทธิ์ของผู้ใช้ Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions)</span><span class="sxs-lookup"><span data-stu-id="75608-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="75608-130">**ฉันมีปัญหาในการใช้พารามิเตอร์คิวรี OData เพื่อกรองข้อมูลในคำขอของฉัน**</span><span class="sxs-lookup"><span data-stu-id="75608-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="75608-131">ในขณะที่ Microsoft Graph สนับสนุนพารามิเตอร์แบบสอบถาม OData หลายพารามิเตอร์เหล่านั้นจะไม่ได้รับการสนับสนุนอย่างสมบูรณ์โดยบริการไดเรกทอรี (แหล่งข้อมูลที่สืบทอดมาจาก *directoryObject*) ใน Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="75608-132">ข้อจำกัดเดียวกันกับที่มีอยู่ในกราฟโฆษณา Azure ได้รับการยืนยันสำหรับส่วนใหญ่ใน Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="75608-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="75608-133">**ไม่ได้รับการสนับสนุน**: $count, $search และ $filter บนค่า *null* หรือ *ไม่ใช่ค่า null*</span><span class="sxs-lookup"><span data-stu-id="75608-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="75608-134">**ไม่ได้รับการสนับสนุน**: $filter บนคุณสมบัติบางอย่าง (โปรดดูที่หัวข้อทรัพยากรที่มีคุณสมบัติใดที่เอา)</span><span class="sxs-lookup"><span data-stu-id="75608-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="75608-135">**ไม่ได้รับการสนับสนุน**: การแบ่งหน้าการกรองและการเรียงลำดับในเวลาเดียวกัน</span><span class="sxs-lookup"><span data-stu-id="75608-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="75608-136">**ไม่ได้รับการสนับสนุน**: การกรองบนความสัมพันธ์</span><span class="sxs-lookup"><span data-stu-id="75608-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="75608-137">ตัวอย่างเช่นค้นหาสมาชิกทั้งหมดของกลุ่มวิศวกรรมที่อยู่ในสหราชอาณาจักร</span><span class="sxs-lookup"><span data-stu-id="75608-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="75608-138">การ **สนับสนุนบางส่วน**: $orderby บน *ผู้ใช้*(displayName และ userPrincipalName เท่านั้น) และ *กลุ่ม*</span><span class="sxs-lookup"><span data-stu-id="75608-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="75608-139">การ **สนับสนุนบางส่วน**: $filter (สนับสนุนเฉพาะ *eq*, startswith *หรือ*, *and และ* จำกัด) การสนับสนุน $expand (การขยายความสัมพันธ์ของวัตถุเดี่ยวจะส่งกลับความสัมพันธ์ทั้งหมดแต่การขยายคอลเลกชันของความสัมพันธ์ของวัตถุจะถูกจำกัด) </span><span class="sxs-lookup"><span data-stu-id="75608-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="75608-140">สำหรับข้อมูลเพิ่มเติมให้ดูที่การกำหนดค่าการ [ตอบสนองด้วยพารามิเตอร์คิว](https://docs.microsoft.com/graph/query-parameters)รี</span><span class="sxs-lookup"><span data-stu-id="75608-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="75608-141">**API ที่ฉันกำลังโทรไม่ทำงาน-ฉันสามารถทำการทดสอบเพิ่มเติมได้จากที่ใด**</span><span class="sxs-lookup"><span data-stu-id="75608-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="75608-142">**Microsoft Graph Explorer** -ทดสอบ Microsoft graph APIs ในผู้เช่าของคุณหรือผู้เช่าสาธิตและยังตรวจสอบ **แบบสอบถามตัวอย่าง** ใน Microsoft Graph explorer</span><span class="sxs-lookup"><span data-stu-id="75608-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="75608-143">**เมื่อฉันทำแบบสอบถามสำหรับข้อมูลดูเหมือนว่าฉันได้รับชุดข้อมูลที่ไม่สมบูรณ์กลับมา**</span><span class="sxs-lookup"><span data-stu-id="75608-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="75608-144">ถ้าคุณกำลังทำการสอบถามคอลเลกชัน (เช่น *ผู้ใช้*) Microsoft Graph จะใช้ขีดจำกัดของหน้าบนเซิร์ฟเวอร์เพื่อให้ผลลัพธ์จะถูกส่งกลับโดยใช้ขนาดหน้าเริ่มต้นเสมอ</span><span class="sxs-lookup"><span data-stu-id="75608-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="75608-145">แอปของคุณควรคาดหวังให้หน้าผ่านคอลเลกชันที่ส่งกลับจากบริการนั้นเสมอ</span><span class="sxs-lookup"><span data-stu-id="75608-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="75608-146">สำหรับข้อมูลเพิ่มเติม ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="75608-146">For more information, see:</span></span>

- [<span data-ttu-id="75608-147">แนวทางปฏิบัติที่ดีที่สุดของ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="75608-148">การแบ่งหน้าข้อมูล Microsoft Graph ในแอปของคุณ</span><span class="sxs-lookup"><span data-stu-id="75608-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="75608-149">**แอปของฉันช้าเกินไปและยังได้รับปริมาณ ฉันสามารถทำการปรับปรุงอะไรได้บ้าง**</span><span class="sxs-lookup"><span data-stu-id="75608-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="75608-150">ทั้งนี้ขึ้นอยู่กับสถานการณ์ของคุณมีหลายตัวเลือกที่แตกต่างกันในการขายทิ้งของคุณเพื่อทำให้แอปพลิเคชันของคุณมีประสิทธิภาพมากขึ้นและในบางกรณีอาจมีแนวโน้มที่จะปริมาณโดยบริการ (เมื่อคุณกำลังทำการโทรมากเกินไป)</span><span class="sxs-lookup"><span data-stu-id="75608-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="75608-151">เมื่อต้องการเรียนรู้เพิ่มเติมให้ดูที่:</span><span class="sxs-lookup"><span data-stu-id="75608-151">To learn more, see:</span></span>

- [<span data-ttu-id="75608-152">แนวทางปฏิบัติที่ดีที่สุดของ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="75608-153">การร้องขอ Batching</span><span class="sxs-lookup"><span data-stu-id="75608-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="75608-154">ติดตามการเปลี่ยนแปลงผ่านคิวรีของเดลต้า</span><span class="sxs-lookup"><span data-stu-id="75608-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="75608-155">รับการแจ้งเตือนการเปลี่ยนแปลงผ่าน webhooks</span><span class="sxs-lookup"><span data-stu-id="75608-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="75608-156">คำแนะนำการควบคุมปริมาณ</span><span class="sxs-lookup"><span data-stu-id="75608-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="75608-157">**ฉันจะค้นหาข้อมูลเพิ่มเติมเกี่ยวกับข้อผิดพลาดและปัญหาที่ทราบได้ที่ไหน**</span><span class="sxs-lookup"><span data-stu-id="75608-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="75608-158">ข้อมูลการตอบกลับข้อผิดพลาดของ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="75608-159">ปัญหาที่ทราบแล้วเกี่ยวกับ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="75608-160">**ฉันจะตรวจสอบสถานะของบริการที่พร้อมใช้งานและการเชื่อมต่อได้ที่ใด**</span><span class="sxs-lookup"><span data-stu-id="75608-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="75608-161">ความพร้อมใช้งานของบริการและการเชื่อมต่อของบริการพื้นฐานที่สามารถเข้าถึงได้ผ่านทาง Microsoft Graph จะส่งผลกระทบต่อความพร้อมใช้งานและประสิทธิภาพการทำงานโดยรวมของ Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="75608-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="75608-162">สำหรับสถานภาพบริการของ Azure Active Directory ให้ตรวจสอบสถานะของ **ความปลอดภัย + บริการข้อมูลประจำตัว** ที่แสดงรายการอยู่ใน [หน้าสถานะ Azure](https://azure.microsoft.com/status/)</span><span class="sxs-lookup"><span data-stu-id="75608-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="75608-163">สำหรับบริการ Office ที่เกี่ยวข้องกับ Microsoft Graph ให้ตรวจสอบสถานะของบริการที่แสดงรายการอยู่ใน[แดชบอร์ดความสมบูรณ์ของบริการ Office](https://portal.office.com/adminportal/home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="75608-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
