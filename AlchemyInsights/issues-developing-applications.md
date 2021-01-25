---
title: ปัญหาในการพัฒนาแอปพลิเคชัน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974765"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="bc9f2-102">ปัญหาในการพัฒนาแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="bc9f2-102">Issues developing applications</span></span>

<span data-ttu-id="bc9f2-103">เมื่อต้องการแก้ไขปัญหาทั่วไปที่พบมากที่สุดเมื่อสร้างแอป Azure Active Directory (AD) ให้ดูบทความต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="bc9f2-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="bc9f2-104">ฉันเห็นปัญหาในการลงชื่อเข้าใช้แอปพลิเคชันโดยใช้เบราว์เซอร์ Chrome เท่านั้น</span><span class="sxs-lookup"><span data-stu-id="bc9f2-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="bc9f2-105">ฉันไม่ทราบวิธีการเปลี่ยนค่าเริ่มต้นตลอดอายุการใช้งานของโทเค็นสำหรับแอปพลิเคชันของฉัน</span><span class="sxs-lookup"><span data-stu-id="bc9f2-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="bc9f2-106">ฉันสับสนเกี่ยวกับวิธีการทำงานของความยินยอมของแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="bc9f2-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="bc9f2-107">ฉันไม่ทราบวิธีการให้สิทธิ์กับแอปพลิเคชันของฉัน</span><span class="sxs-lookup"><span data-stu-id="bc9f2-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="bc9f2-108">ฉันไม่เข้าใจความแตกต่างระหว่างสิทธิ์ที่มอบหมายและแอปพลิเคชัน</span><span class="sxs-lookup"><span data-stu-id="bc9f2-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="bc9f2-109">\***จุดสิ้นสุดของการสนับสนุนสำหรับ Azure Active Directory ไลบรารีการรับรองความถูกต้อง (ADAL) และ AZURE AD graph (graph)** _</span><span class="sxs-lookup"><span data-stu-id="bc9f2-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="bc9f2-110">เริ่มต้นวันที่30มิถุนายน๒๐๒๐เราจะไม่เพิ่มฟีเจอร์ใหม่อีกต่อไปในไลบรารีการรับรองความถูกต้องของ Azure Active Directory (ADAL) และ Azure AD Graph (Graph Graph)</span><span class="sxs-lookup"><span data-stu-id="bc9f2-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="bc9f2-111">เราจะยังคงให้การสนับสนุนทางเทคนิคและการอัปเดตความปลอดภัยแต่จะไม่มีการอัปเดตของฟีเจอร์อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="bc9f2-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="bc9f2-112">เริ่มต้นวันที่30มิถุนายน๒๐๒๒เราจะสิ้นสุดการสนับสนุนสำหรับ ADAL และ AAD กราฟและจะไม่ให้การสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="bc9f2-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="bc9f2-113">ผลลัพธ์ของเงื่อนไขนี้จะมีผลกระทบต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="bc9f2-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="bc9f2-114">แอปที่ใช้ ADAL บน OS เวอร์ชันที่มีอยู่จะยังคงทำงานต่อไปหลังจากเวลานี้แต่จะไม่ได้รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="bc9f2-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="bc9f2-115">แอปที่ใช้กราฟ AAD หลังจากเวลานี้อาจไม่ได้รับการตอบสนองจากจุดสิ้นสุดของกราฟ AAD</span><span class="sxs-lookup"><span data-stu-id="bc9f2-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="bc9f2-116">การ *โยกย้าย _ ADAL*\*</span><span class="sxs-lookup"><span data-stu-id="bc9f2-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="bc9f2-117">ถ้าคุณกำลังใช้แอป Microsoft เราขอแนะนำให้อัปเดตเป็นไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL) ซึ่งมีฟีเจอร์และการอัปเดตความปลอดภัยล่าสุด</span><span class="sxs-lookup"><span data-stu-id="bc9f2-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="bc9f2-118">คำแนะนำนี้อยู่ในบริบทของ Microsoft ในการเริ่มต้นกระบวนการโยกย้ายแอปของแอปไปยัง MSAL โดยกำหนดเวลาสิ้นสุดของการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="bc9f2-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="bc9f2-119">การโยกย้ายโดยไมโครซอฟท์ของแอ MSAL เพื่อให้แน่ใจว่าแอปจะได้รับประโยชน์จากการปรับปรุงความปลอดภัยและฟีเจอร์ที่ต่อเนื่องของ MSAL</span><span class="sxs-lookup"><span data-stu-id="bc9f2-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="bc9f2-120">อ่านคำถามที่ถามบ่อยเกี่ยวกับ ADAL</span><span class="sxs-lookup"><span data-stu-id="bc9f2-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="bc9f2-121">เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปบนไซต์ต่อเนื่อง</span><span class="sxs-lookup"><span data-stu-id="bc9f2-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="bc9f2-122">ถ้าคุณต้องการความช่วยเหลือในการทำความเข้าใจที่แอปของคุณใช้ ADAL เราขอแนะนำให้คุณตรวจทานโค้ดต้นฉบับของแอพทั้งหมดของคุณและถ้ามีให้ติดต่อผู้จำหน่ายซอฟต์แวร์อิสระ (Isv) หรือผู้ให้บริการแอป</span><span class="sxs-lookup"><span data-stu-id="bc9f2-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="bc9f2-123">ฝ่ายสนับสนุนของ microsoft ยังสามารถให้คุณมีรายการของแอป ADAL ที่ไม่ใช่ Microsoft ทั้งหมดในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="bc9f2-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="bc9f2-124">**การโยกย้ายกราฟ AAD**</span><span class="sxs-lookup"><span data-stu-id="bc9f2-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="bc9f2-125">สำหรับแอปพลิเคชันที่ใช้กราฟ AAD ให้ทำตามคำแนะนำของเราในการโยกย้ายแอปการใช้กราฟ AAD ไปยัง Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="bc9f2-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="bc9f2-126">[รายการตรวจสอบการโยกย้ายของเรามีจุดเริ่มต้นใช้](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)งาน</span><span class="sxs-lookup"><span data-stu-id="bc9f2-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="bc9f2-127">พอร์ทัลการลงทะเบียนแอ Azure ของคุณแสดงแอปพลิเคชันที่ใช้กราฟ AAD</span><span class="sxs-lookup"><span data-stu-id="bc9f2-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="bc9f2-128">เราขอแนะนำให้คุณตรวจทานโค้ดต้นฉบับของแอปของคุณทั้งหมดและถ้ามีผลบังคับให้ติดต่อผู้จำหน่ายซอฟต์แวร์อิสระ (Isv) หรือผู้ให้บริการแอป</span><span class="sxs-lookup"><span data-stu-id="bc9f2-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="bc9f2-129">ฝ่ายสนับสนุนของ Microsoft ยังสามารถให้ข้อมูลเกี่ยวกับการใช้งานของการใช้กราฟ AAD ในผู้เช่าของคุณได้อีกด้วย</span><span class="sxs-lookup"><span data-stu-id="bc9f2-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







