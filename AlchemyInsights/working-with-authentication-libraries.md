---
title: การใช้งานได้กับไลบรารีการรับรองความถูกต้อง
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036866"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="04014-102">การใช้งานได้กับไลบรารีการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="04014-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="04014-103">เมื่อต้องการแก้ไขปัญหา Microsoft Authentication Library (MSAL) ให้ปฏิบัติตามขั้นตอนที่แนะนาต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="04014-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="04014-104">**การแก้ไขข้อผิดพลาด MSAL**: [ไลบรารีการรับรองความถูกต้องแพลตฟอร์ม](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) ข้อมูลเฉพาะตัวของ Microsoft - บทความนี้แสดงการสนับสนุนไลบรารีการรับรองความถูกต้องของ Microsoft ชนิดของแอปพลิเคชันหลายชนิด</span><span class="sxs-lookup"><span data-stu-id="04014-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="04014-105">It includes links to library source code; จะรับแพคเกจของโครงการแอปได้ที่ไหน และไลบรารีสนับสนุนการลงชื่อเข้าใช้ (การรับรองความถูกต้อง) ของผู้ใช้ การเข้าถึง API (การอนุญาต) เว็บที่มีการป้องกัน หรือทั้งสองอย่าง</span><span class="sxs-lookup"><span data-stu-id="04014-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="04014-106">**แก้ไขปัญหาการรับรองความถูก** ต้อง: MSAL สนับสนุนขั้นตอนการรับรองความถูกต้องหลายอย่างเพื่อใช้ในสถานการณ์ของแอปพลิเคชันต่างๆ</span><span class="sxs-lookup"><span data-stu-id="04014-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="04014-107">MSAL สามารถใช้ขั้นตอนการรับรองความถูกต้องอย่างน้อยหนึ่งรายการที่สนับสนุนโดยแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft ทั้งนี้ขึ้นอยู่กับวิธีการสร้างแอปพลิเคชันไคลเอ็นต์ของคุณ</span><span class="sxs-lookup"><span data-stu-id="04014-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="04014-108">ขั้นตอนเหล่านี้สามารถสร้างโทเค็นและรหัสการอนุญาตหลายชนิด และต้องใช้โทเค็นที่แตกต่างกันเพื่อใช้งาน</span><span class="sxs-lookup"><span data-stu-id="04014-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="04014-109">**เข้าถึงโทเค็น**: [โทเค็นการเข้าถึงแพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - เรียนรู้วิธีที่ API ของคุณสามารถตรวจสอบและใช้การอ้างสิทธิ์ภายในโทเค็นการเข้าถึง</span><span class="sxs-lookup"><span data-stu-id="04014-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="04014-110">เอกสารประกอบทั้งหมดในบทความนี้ ยกเว้นตามบันทึกที่บันทึกจะใช้ได้กับโทเค็นที่ออกให้กับ API ที่คุณได้ลงทะเบียนเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="04014-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="04014-111">ซึ่งจะไม่มีผลบังคับใช้กับโทเค็นที่ออกให้กับ API ที่ Microsoft เป็นเจ้าของ และไม่สามารถใช้โทเค็นเหล่านั้นเพื่อตรวจสอบความถูกต้องของวิธีที่แพลตฟอร์มข้อมูลเฉพาะตัวของ Microsoft จะออกโทเค็นให้กับ API ที่คุณสร้าง</span><span class="sxs-lookup"><span data-stu-id="04014-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="04014-112">**การสิ้นสุดการสนับสนุนของ Azure Active Directory Authentication Library (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="04014-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="04014-113">**ตั้งแต่วันที่ 30 มิถุนายน 2020** เราจะไม่เพิ่มฟีเจอร์ใหม่ใดๆ ลงใน ADAL และ Azure AD Graph อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="04014-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="04014-114">เราจะให้การสนับสนุนด้านเทคนิคและการอัปเดตความปลอดภัยต่อ แต่จะไม่มีการอัปเดตฟีเจอร์อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="04014-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="04014-115">**ตั้งแต่วันที่ 30 มิถุนายน 2022** เราจะสิ้นสุดการสนับสนุน ADAL และ Azure AD Graph และจะไม่มีการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="04014-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="04014-116">แอปที่ใช้ ADAL บนเวอร์ชัน OS ที่มีอยู่จะยังคงสามารถใช้งานต่อไปได้หลังจากนี้ *แต่จะไม่ได้รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัย* ใดๆ</span><span class="sxs-lookup"><span data-stu-id="04014-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="04014-117">แอปที่ใช้ Azure AD Graph หลังจากช่วงเวลานี้อาจไม่ได้รับการตอบกลับจากจุดสิ้นสุด Azure AD Graph อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="04014-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="04014-118">**การโยกย้าย ADAL**</span><span class="sxs-lookup"><span data-stu-id="04014-118">**ADAL Migration**</span></span>

- <span data-ttu-id="04014-119">เราขอแนะนนะให้อัปเดตเป็น MSAL ซึ่งมีฟีเจอร์และการอัปเดตความปลอดภัยล่าสุด</span><span class="sxs-lookup"><span data-stu-id="04014-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="04014-120">ถ้าคุณใช้งานแอป Microsoft ทราบว่า Microsoft อยู่ในระหว่างการโยกย้ายแอปไปยัง MSAL ภายในวันสิ้นสุดการสนับสนุน เพื่อให้มั่นใจว่าพวกเขาจะได้รับประโยชน์จากการรักษาความปลอดภัยและการปรับปรุงฟีเจอร์ที่ MSAL มีอย่างต่อเนื่อง</span><span class="sxs-lookup"><span data-stu-id="04014-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="04014-121">[อ่าน ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="04014-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="04014-122">[เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปตามแพลตฟอร์ม](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)</span><span class="sxs-lookup"><span data-stu-id="04014-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="04014-123">ถ้าหลังจากอ่านคู่มือแพลตฟอร์มของแอปของคุณคุณมีข้อถามเพิ่มเติม คุณสามารถโพสต์บนถามตอบของ Microsoft [Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) ที่มีแท็ก [azure-ad-adal-deprecation] หรือเปิดปัญหาในที่เก็บ GitHub ของไลบรารี</span><span class="sxs-lookup"><span data-stu-id="04014-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="04014-124">ดู [ส่วนภาษาและ](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) เฟรมเวิร์กของ **บทความภาพรวม MSAL** เพื่อลิงก์ไปยังการ repo ของไลบรารีแต่ละรายการ</span><span class="sxs-lookup"><span data-stu-id="04014-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="04014-125">**ถ้าคุณต้องการความช่วยเหลือในการเข้าใจว่าแอปใดของคุณใช้ ADAL** เราขอแนะนนะให้คุณตรวจสอบโค้ดต้นฉบับของแอปทั้งหมด</span><span class="sxs-lookup"><span data-stu-id="04014-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="04014-126">ถ้าสามารถติดต่อผู้ขายซอฟต์แวร์อิสระ (ISVs) หรือผู้ให้บริการแอป</span><span class="sxs-lookup"><span data-stu-id="04014-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="04014-127">ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการของแอปที่ไม่ใช่ Microsoft ADAL ทั้งหมดในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="04014-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







