---
title: แอปการรับรองความถูกต้อง
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405683"
---
# <a name="authentication-app"></a><span data-ttu-id="604ba-102">แอปการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="604ba-102">Authentication app</span></span>

<span data-ttu-id="604ba-103">ถ้าคุณเป็นผู้ดูแลระบบส่วนกลาง คุณสามารถค้นหาสิ่งที่เกิดขึ้นหรือวินิจฉัยปัญหาที่เกี่ยวข้องกับการลงชื่อเข้าใช้ของผู้ใช้ได้อย่างรวดเร็วโดยใช้ [การวินิจฉัยการ](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)ลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="604ba-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="604ba-104">เริ่มการวินิจฉัยโดยคลิกปุ่ม "[เปิดใช้การวินิจฉัย](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)"</span><span class="sxs-lookup"><span data-stu-id="604ba-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="604ba-105">ค้นหาเหตุการณ์ที่จะวิเคราะห์โดยการใส่รายละเอียดที่คุณมีเกี่ยวกับผู้ใช้ แอปพลิเคชัน เวลาลงชื่อเข้าใช้ ID การร้องขอ หรือ ID สหสัมพันธ์</span><span class="sxs-lookup"><span data-stu-id="604ba-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="604ba-106">ตรวจทานผลลัพธ์การวินิจฉัยซึ่งแสดงรายละเอียดของสิ่งที่เกิดขึ้นและการดําเนินการที่คุณสามารถดําเนินการเพื่อเปลี่ยนแปลงได้ ถ้ามีการเปลี่ยนแปลงใดๆ ที่ต้องใช้</span><span class="sxs-lookup"><span data-stu-id="604ba-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="604ba-107">**ตรวจสอบสถานการณ์สมมติที่เกี่ยวข้อง:**</span><span class="sxs-lookup"><span data-stu-id="604ba-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="604ba-108">ถ้าผู้ใช้ไม่ได้รับการแจ้งเตือนแบบพุชในแอป Microsoft Authenticator ให้ตรวจสอบว่าไม่ได้แสดงอยู่ภายใต้ผู้ใช้ที่ถูกบล็อก MFA ตามที่อธิบายไว้ในการบล็อกและยกเลิกการ[บล็อกผู้ใช้](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="604ba-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="604ba-109">ถ้าผู้ใช้ไม่ถูกบล็อกด้วย MFA แต่ไม่ได้รับการแจ้งเตือนแบบพุช พวกเขาจะสามารถเปิดแอป Microsoft Authenticator ซึ่งจะดึงการร้องขอการอนุมัติที่ค้างอยู่</span><span class="sxs-lookup"><span data-stu-id="604ba-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="604ba-110">ในฐานะที่เป็นวิธีการลงชื่อเข้าใช้อื่น ผู้ใช้ยังสามารถคลิกลงชื่อเข้าใช้ด้วยวิธีอื่นและเลือกใช้รหัสการตรวจสอบจากแอปบนอุปกรณ์เคลื่อนที่ของฉัน</span><span class="sxs-lookup"><span data-stu-id="604ba-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="604ba-111">แอป Microsoft Authenticator คือวิธีที่พร้อมใช้งานเฉพาะผู้ใช้หลายคนเท่านั้น</span><span class="sxs-lookup"><span data-stu-id="604ba-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="604ba-112">[เรียนรู้เพิ่มเติมเกี่ยวกับค่าเริ่มต้นด้านความปลอดภัย ตรวจสอบ Faq](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)[ของแอป Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq)เพื่อดูข้อถามที่ถามบ่อยและวิธีการแก้ไข</span><span class="sxs-lookup"><span data-stu-id="604ba-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="604ba-113">**วิดีโอที่แนะนนะ**</span><span class="sxs-lookup"><span data-stu-id="604ba-113">**Recommended Videos**</span></span>

<span data-ttu-id="604ba-114">[วิธีการตั้งค่าแอป Authenticator บนโทรศัพท์เครื่องใหม่ (2 นาที)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="604ba-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
