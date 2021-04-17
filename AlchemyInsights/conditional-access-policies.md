---
title: นโยบายการเข้าถึงตามเงื่อนไข
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817299"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="c738b-102">นโยบายการเข้าถึงตามเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="c738b-102">Conditional Access policies</span></span>

<span data-ttu-id="c738b-103">การเข้าถึงตามเงื่อนไขคือความสามารถของ Azure AD ที่ช่วยให้คุณบังคับใช้การควบคุมการเข้าถึงแอปในสภาพแวดล้อมของคุณ ทั้งหมดจะยึดตามเงื่อนไขที่เฉพาะเจาะจงและจัดการจากศูนย์กลาง</span><span class="sxs-lookup"><span data-stu-id="c738b-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="c738b-104">เรียนรู้เพิ่มเติมเกี่ยวกับ[การเข้าถึงตามเงื่อนไขของ Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/)</span><span class="sxs-lookup"><span data-stu-id="c738b-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="c738b-105">**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่ 21 ตุลาคม 2019 และคุณได้รับพร้อมท์โดยไม่คาดคิดเกี่ยวกับ MFA คุณอาจเปิดใช้งานค่าเริ่มต้นด้านความปลอดภัยใน [](https://aka.ms/securitydefaults)ผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="c738b-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="c738b-106">**เมื่อต้องการจัดการค่าเริ่มต้นความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="c738b-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="c738b-107">ลงชื่อเข้าใช้ศูนย์การจัดการ [ด้วยข้อมูล](https://go.microsoft.com/fwlink/p/?linkid=834822) รับรองความถูกต้องของผู้ดูแลระบบส่วนกลางของคุณ</span><span class="sxs-lookup"><span data-stu-id="c738b-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="c738b-108">ไปที่[คุณสมบัติ Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)</span><span class="sxs-lookup"><span data-stu-id="c738b-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="c738b-109">ที่ด้านล่างของหน้า ให้คลิก **จัดการค่าเริ่มต้นความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="c738b-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="c738b-110">คลิกใช่ เพื่อเปิดใช้งานค่าเริ่มต้นความปลอดภัย **หรือ** ไม่ใช่ เพื่อปิดใช้งานค่าเริ่มต้นด้านความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="c738b-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
