---
title: ปัญหาเกี่ยวกับไลบรารีการรับรองความถูกต้อง
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063701"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="86578-102">ปัญหาเกี่ยวกับไลบรารีการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="86578-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="86578-103">[ไลบรารีการรับรองความถูกต้องแพลตฟอร์มข้อมูลเฉพาะตัวของ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) Microsoft แสดงรายการไลบรารีไคลเอ็นต์และ Middleware ที่ได้รับการสนับสนุนและเข้ากันได้ของ Microsoft</span><span class="sxs-lookup"><span data-stu-id="86578-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="86578-104">ไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL) สนับสนุนขั้นตอน [การรับรองความถูกต้องหลายอย่าง](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) เพื่อใช้ในสถานการณ์ของแอปพลิเคชันต่างๆ</span><span class="sxs-lookup"><span data-stu-id="86578-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="86578-105">เมื่อต้องการรับรองความถูกต้องและรับโทเค็น ให้คุณเตรียมใช้งานแอปพลิเคชันไคลเอ็นต์สาธารณะหรือแอปพลิเคชันที่เป็นความลับใหม่ในโค้ดของคุณ</span><span class="sxs-lookup"><span data-stu-id="86578-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="86578-106">คุณสามารถตั้งค่าตัวเลือกการกําหนดค่าได้หลายตัวเลือกเมื่อคุณเตรียมใช้งานแอปไคลเอ็นต์ในไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL)</span><span class="sxs-lookup"><span data-stu-id="86578-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="86578-107">เมื่อต้องการเรียนรู้เพิ่มเติม ดูตัวเลือก [การกําหนดค่า](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)แอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="86578-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="86578-108">**การสิ้นสุดการสนับสนุนของ Azure Active Directory Authentication Library (ADAL) และ Azure AD Graph API (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="86578-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="86578-109">**ตั้งแต่วันที่ 30 มิถุนายน 2020** เราจะไม่เพิ่มฟีเจอร์ใหม่ใดๆ ลงใน ADAL และ Azure AD Graph อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="86578-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="86578-110">เราจะให้การสนับสนุนด้านเทคนิคและการอัปเดตความปลอดภัยต่อ แต่จะไม่มีการอัปเดตฟีเจอร์อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="86578-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="86578-111">**ตั้งแต่วันที่ 30 มิถุนายน 2022** เราจะสิ้นสุดการสนับสนุน ADAL และ Azure AD Graph และจะไม่มีการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="86578-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="86578-112">แอปที่ใช้ ADAL บนเวอร์ชัน OS ที่มีอยู่จะยังคงสามารถใช้งานต่อไปได้หลังจากนี้ *แต่จะไม่ได้รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัย* ใดๆ</span><span class="sxs-lookup"><span data-stu-id="86578-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="86578-113">แอปที่ใช้ Azure AD Graph หลังจากช่วงเวลานี้อาจไม่ได้รับการตอบกลับจากจุดสิ้นสุด Azure AD Graph อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="86578-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="86578-114">**การโยกย้าย ADAL**</span><span class="sxs-lookup"><span data-stu-id="86578-114">**ADAL Migration**</span></span>

<span data-ttu-id="86578-115">เราขอแนะนนะ [ให้อัปเดตไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)ซึ่งมีฟีเจอร์ล่าสุดและการอัปเดตความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="86578-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="86578-116">ถ้าคุณใช้งานแอปของ Microsoft ทราบว่า Microsoft อยู่ในระหว่างกระบวนการโยกย้ายแอปพลิเคชันไปยัง MSAL ภายในวันที่สิ้นสุดการสนับสนุน เพื่อให้มั่นใจว่าแอปเหล่านั้นจะได้รับประโยชน์จากการรักษาความปลอดภัยและการปรับปรุงฟีเจอร์ที่ MSAL อย่างต่อเนื่อง</span><span class="sxs-lookup"><span data-stu-id="86578-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="86578-117">สำหรับข้อมูลเพิ่มเติม ให้ดูที่</span><span class="sxs-lookup"><span data-stu-id="86578-117">For more information, see:</span></span>

1. [<span data-ttu-id="86578-118">อ่าน ADAL FAQ</span><span class="sxs-lookup"><span data-stu-id="86578-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="86578-119">เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปตามแพลตฟอร์ม</span><span class="sxs-lookup"><span data-stu-id="86578-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="86578-120">ถ้าคุณต้องการความช่วยเหลือในการเข้าใจว่าแอปใดของคุณใช้ ADAL เราขอแนะนาให้คุณตรวจสอบโค้ดต้นฉบับของแอปของคุณทั้งหมด และถ้าสามารถใช้งานได้ ให้ติดต่อผู้ให้บริการ ISVs หรือแอปรายใดก็ได้</span><span class="sxs-lookup"><span data-stu-id="86578-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="86578-121">ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการของแอปที่ไม่ใช่ Microsoft ADAL ทั้งหมดในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="86578-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="86578-122">**การโยกย้ายกราฟ AAD**</span><span class="sxs-lookup"><span data-stu-id="86578-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="86578-123">สําหรับแอปพลิเคชันที่ใช้ Azure AD Graph ให้ปฏิบัติตามแนวทางของเราเพื่อ[โยกย้ายแอป Azure AD Graph ไปยัง Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)</span><span class="sxs-lookup"><span data-stu-id="86578-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="86578-124">รายการตรวจสอบการโยกย้ายของเราให้จุดเริ่มต้น</span><span class="sxs-lookup"><span data-stu-id="86578-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="86578-125">พอร์ทัลการลงทะเบียนแอป Azure ของคุณจะแสดงแอปพลิเคชันที่ใช้ AAD Graph</span><span class="sxs-lookup"><span data-stu-id="86578-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="86578-126">เราขอแนะนนะให้คุณตรวจสอบรหัสต้นฉบับของแอปของคุณทั้งหมด และหากสามารถติดต่อผู้ให้บริการ ISVs หรือแอปใดก็ได้</span><span class="sxs-lookup"><span data-stu-id="86578-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="86578-127">ฝ่ายสนับสนุนของ Microsoft ยังสามารถแสดงรายการการใช้งาน AAD Graph ทั้งหมดในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="86578-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="86578-128">เพื่อให้แอปของคุณเข้าถึงข้อมูลใน Microsoft Graph ผู้ใช้หรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการการยินยอม</span><span class="sxs-lookup"><span data-stu-id="86578-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="86578-129">การอ้างอิง [สิทธิ์ของ Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับแต่ละชุดหลักของ Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="86578-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="86578-130">นอกจากนี้ยังมีแนวทางเกี่ยวกับวิธีการใช้สิทธิ์</span><span class="sxs-lookup"><span data-stu-id="86578-130">It also provides guidance about how to use the permissions.</span></span>
