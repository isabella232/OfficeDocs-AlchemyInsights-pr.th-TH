---
title: ปัญหาเกี่ยวกับการเข้าถึงตามเงื่อนไข
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
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015004"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="78d41-102">ปัญหาเกี่ยวกับการเข้าถึงตามเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="78d41-102">Conditional access issues</span></span>

<span data-ttu-id="78d41-103">**แก้ไขปัญหาเกี่ยวกับการวินิจฉัยการเข้าสู่ระบบ**</span><span class="sxs-lookup"><span data-stu-id="78d41-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="78d41-104">คุณสามารถค้นหาสิ่งที่เกิดขึ้นหรือวินิจฉัยปัญหาที่เกี่ยวข้องกับการลงชื่อเข้าใช้ของผู้ใช้โดยใช้การ [วินิจฉัยการเข้าสู่ระบบ](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)ได้อย่างรวดเร็ว:</span><span class="sxs-lookup"><span data-stu-id="78d41-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="78d41-105">เปิดใช้งานการวินิจฉัยการลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="78d41-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="78d41-106">ค้นหาเหตุการณ์ในการวิเคราะห์โดยการใส่รายละเอียดที่คุณมีเกี่ยวกับผู้ใช้แอปพลิเคชันเวลาของการลงชื่อเข้าใช้ Id คำขอหรือ Id สหสัมพันธ์</span><span class="sxs-lookup"><span data-stu-id="78d41-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="78d41-107">ตรวจทานผลลัพธ์การวินิจฉัยแสดงรายละเอียดของสิ่งที่เกิดขึ้นและการดำเนินการที่คุณสามารถทำได้เพื่อทำการเปลี่ยนแปลง (ถ้าจำเป็นต้องมีการเปลี่ยนแปลง)</span><span class="sxs-lookup"><span data-stu-id="78d41-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="78d41-108">**ขั้นตอนในการแก้ไขปัญหาการลงชื่อเข้าใช้**</span><span class="sxs-lookup"><span data-stu-id="78d41-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="78d41-109">นำทางไปยังหน้าการลงชื่อเข้าใช้ Azure AD</span><span class="sxs-lookup"><span data-stu-id="78d41-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="78d41-110">ตัวกรองการลงชื่อเข้าใช้โดยผู้ใช้ช่วงเวลาแอปพลิเคชันสถานะแอปพลิเคชันไคลเอ็นต์และอื่นๆ</span><span class="sxs-lookup"><span data-stu-id="78d41-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="78d41-111">เลือกเหตุการณ์การลงชื่อเข้าใช้และดูแท็บการเข้าถึงแบบมีเงื่อนไขเพื่อดูว่านโยบายใดที่ได้รับการประเมิน</span><span class="sxs-lookup"><span data-stu-id="78d41-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="78d41-112">คลิกแถวของนโยบายเพื่อดูรายละเอียดนโยบายและทำความเข้าใจว่าทำไมจึงนำไปใช้</span><span class="sxs-lookup"><span data-stu-id="78d41-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="78d41-113">**เครื่องมือในการแก้ไขปัญหานโยบายการเข้าถึงแบบมีเงื่อนไข**</span><span class="sxs-lookup"><span data-stu-id="78d41-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="78d41-114">โหมดรายงานเท่านั้นให้คุณประเมินนโยบายโดยไม่มีผลกระทบต่อผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="78d41-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="78d41-115">เครื่องมืออะไรที่ช่วยให้คุณสามารถจำลองเหตุการณ์การลงชื่อเข้าใช้และดูว่ามีการนำนโยบายไปใช้</span><span class="sxs-lookup"><span data-stu-id="78d41-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="78d41-116">เวิร์กบุ๊กข้อมูลเชิงลึกและการรายงานจะแสดงผลกระทบแบบเรียลไทม์ของนโยบายแต่ละรายการ</span><span class="sxs-lookup"><span data-stu-id="78d41-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="78d41-117">**นโยบายการป้องกันพื้นฐาน**</span><span class="sxs-lookup"><span data-stu-id="78d41-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="78d41-118">นโยบายการป้องกันพื้นฐานได้รับการสนับสนุน</span><span class="sxs-lookup"><span data-stu-id="78d41-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="78d41-119">พวกเขาจะไม่ถูกบังคับใช้อีกต่อไปและจะถูกเอาออกจากพอร์ทัล Azure ในเร็วๆนี้</span><span class="sxs-lookup"><span data-stu-id="78d41-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="78d41-120">เราขอแนะนำให้เปิดใช้งาน[ค่าเริ่มต้นด้านความปลอดภัย](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="78d41-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="78d41-121">สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงแบบมีเงื่อนไขให้ดู:</span><span class="sxs-lookup"><span data-stu-id="78d41-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="78d41-122">[หลักปฏิบัติที่ดีที่สุดสำหรับการเข้าถึงแบบมีเงื่อนไขใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [เงื่อนไขในการเข้าถึง](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 ตามเงื่อนไข [ตัวควบคุมในการเข้าถึง](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 แบบมีเงื่อนไข [ตำแหน่งที่ตั้งในการเข้าถึง](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)แบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="78d41-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
