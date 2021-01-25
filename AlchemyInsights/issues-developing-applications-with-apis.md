---
title: ปัญหาในการพัฒนาแอปพลิเคชันด้วย APIs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975020"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="52003-102">ปัญหาในการพัฒนาแอปพลิเคชันด้วย APIs</span><span class="sxs-lookup"><span data-stu-id="52003-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="52003-103">เมื่อต้องการเริ่มต้นใช้งาน API กราฟของ Active Directory ของ Azure ให้ดูที่คู่มือการอ้างอิงของ azure [Ad graph quickstart](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) หรือดู [เอกสารอ้างอิงการอ้างอิง API ของ azure ad](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)ของ azure แบบโต้ตอบ</span><span class="sxs-lookup"><span data-stu-id="52003-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="52003-104">**การสิ้นสุดการสนับสนุนสำหรับ Azure Active Directory ไลบรารีการรับรองความถูกต้อง (ADAL) และ Azure AD Graph (Graph Graph)**</span><span class="sxs-lookup"><span data-stu-id="52003-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="52003-105">**เริ่มต้นวันที่30มิถุนายน๒๐๒๐** เราจะไม่เพิ่มฟีเจอร์ใหม่ให้กับกราฟ ADAL และ Azure AD อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="52003-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="52003-106">เราจะยังคงให้การสนับสนุนทางเทคนิคและการอัปเดตความปลอดภัยแต่จะไม่มีการอัปเดตของฟีเจอร์อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="52003-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="52003-107">**เริ่มต้นวันที่30มิถุนายน๒๐๒๒** เราจะสิ้นสุดการสนับสนุนสำหรับ ADAL และ Azure AD Graph และจะไม่มีการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัยอีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="52003-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="52003-108">แอปที่ใช้ ADAL บน OS เวอร์ชันที่มีอยู่จะยังคงทำงานต่อไปหลังจากเวลานี้แต่จะไม่ได้รับการสนับสนุนทางเทคนิคหรือการอัปเดตความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="52003-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="52003-109">แอปที่ใช้กราฟโฆษณา Azure หลังจากเวลานี้อาจไม่ได้รับการตอบกลับจากจุดสิ้นสุดของกราฟ AD Azure อีกต่อไป</span><span class="sxs-lookup"><span data-stu-id="52003-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="52003-110">**การโยกย้าย ADAL**</span><span class="sxs-lookup"><span data-stu-id="52003-110">**ADAL Migration**</span></span>

<span data-ttu-id="52003-111">เราขอแนะนำให้อัปเดตเป็น [ไลบรารีการรับรองความถูกต้องของ Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)ซึ่งมีฟีเจอร์และการอัปเดตความปลอดภัยล่าสุด</span><span class="sxs-lookup"><span data-stu-id="52003-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="52003-112">ถ้าคุณกำลังใช้แอป Microsoft ให้ทราบว่า Microsoft อยู่ในระหว่างการโยกย้ายแอปพลิเคชันของแอปพลิเคชันไปยัง MSAL ตามกำหนดเวลาสิ้นสุดของการสนับสนุนเพื่อให้แน่ใจว่าพวกเขาจะได้รับประโยชน์จากการปรับปรุงความปลอดภัยและฟีเจอร์ที่ต่อเนื่องของ MSAL</span><span class="sxs-lookup"><span data-stu-id="52003-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="52003-113">[อ่านคำถามที่ถามบ่อยเกี่ยวกับ ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="52003-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="52003-114">[เรียนรู้เกี่ยวกับวิธีการโยกย้ายแอปบนไซต์สำหรับแต่ละแพลตฟอร์ม](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)</span><span class="sxs-lookup"><span data-stu-id="52003-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="52003-115">ถ้าคุณต้องการความช่วยเหลือในการทำความเข้าใจเกี่ยวกับแอปที่คุณใช้ ADAL เราขอแนะนำให้คุณตรวจทานโค้ดต้นฉบับของแอพทั้งหมดของคุณและถ้ามีให้เข้าถึง Isv หรือผู้ให้บริการแอป</span><span class="sxs-lookup"><span data-stu-id="52003-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="52003-116">ฝ่ายสนับสนุนของ microsoft ยังสามารถให้คุณมีรายการของแอป ADAL ที่ไม่ใช่ Microsoft ทั้งหมดในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="52003-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="52003-117">**การโยกย้ายกราฟ AAD**</span><span class="sxs-lookup"><span data-stu-id="52003-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="52003-118">สำหรับแอปพลิเคชันที่ใช้กราฟโฆษณา Azure ให้ทำตามคำแนะนำของเราในการโยกย้าย[แอป AZURE AD graph ไปยัง Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="52003-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="52003-119">[รายการตรวจสอบการโยกย้ายของเรามีจุดเริ่มต้นใช้](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)งาน</span><span class="sxs-lookup"><span data-stu-id="52003-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="52003-120">พอร์ทัลการลงทะเบียนแอ Azure ของคุณแสดงแอปพลิเคชันที่ใช้กราฟ AAD</span><span class="sxs-lookup"><span data-stu-id="52003-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="52003-121">เราขอแนะนำให้คุณตรวจทานโค้ดต้นฉบับของแอปของคุณทั้งหมดและถ้ามีผลบังคับให้ติดต่อกับ Isv หรือผู้ให้บริการแอป</span><span class="sxs-lookup"><span data-stu-id="52003-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="52003-122">ฝ่ายสนับสนุนของ Microsoft ยังสามารถให้คุณมีรายการของการใช้งานการใช้กราฟ AAD ทั้งหมดในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="52003-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="52003-123">สำหรับแอปของคุณเพื่อเข้าถึงข้อมูลใน Microsoft Graph ผู้ใช้หรือผู้ดูแลระบบต้องให้สิทธิ์ที่ถูกต้องผ่านทางกระบวนการยินยอม</span><span class="sxs-lookup"><span data-stu-id="52003-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="52003-124">การ [อ้างอิงสิทธิ์ของ Microsoft graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) จะแสดงรายการสิทธิ์ที่เกี่ยวข้องกับชุดหลักของ Microsoft graph APIs แต่ละชุด</span><span class="sxs-lookup"><span data-stu-id="52003-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="52003-125">นอกจากนี้ยังมีคำแนะนำเกี่ยวกับวิธีการใช้สิทธิ์</span><span class="sxs-lookup"><span data-stu-id="52003-125">It also provides guidance about how to use the permissions.</span></span>
