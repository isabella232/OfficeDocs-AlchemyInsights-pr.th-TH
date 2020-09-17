---
title: นโยบายการเข้าถึงแบบมีเงื่อนไข
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 25dc98397920e4fbf28895f5961f154381e11c92
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812278"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="7347c-102">นโยบายการเข้าถึงแบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="7347c-102">Conditional Access policies</span></span>

<span data-ttu-id="7347c-103">การเข้าถึงตามเงื่อนไขคือความสามารถของ Azure AD ที่ช่วยให้คุณสามารถบังคับใช้ตัวควบคุมในการเข้าถึงแอปในสภาพแวดล้อมของคุณโดยยึดตามเงื่อนไขที่เฉพาะเจาะจงและมีการจัดการจากตำแหน่งที่ตั้งส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="7347c-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="7347c-104">เรียนรู้เพิ่มเติมเกี่ยวกับการ[เข้าถึงแบบมีเงื่อนไขของ AZURE AD](https://docs.microsoft.com/azure/active-directory/conditional-access/)</span><span class="sxs-lookup"><span data-stu-id="7347c-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="7347c-105">**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่21ตุลาคม๒๐๑๙และคุณจะได้รับพร้อมท์สำหรับ MFA โดยไม่คาดคิดคุณอาจมี [ค่าเริ่มต้นของความปลอดภัย](https://aka.ms/securitydefaults) ที่เปิดใช้งานในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="7347c-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="7347c-106">**เมื่อต้องการจัดการค่าเริ่มต้นด้านความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="7347c-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="7347c-107">ลงชื่อเข้าใช้ [ศูนย์การจัดการ](https://go.microsoft.com/fwlink/p/?linkid=834822) ด้วยข้อมูลประจำตัวของผู้ดูแลระบบส่วนกลางของคุณ</span><span class="sxs-lookup"><span data-stu-id="7347c-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="7347c-108">ไปยัง [คุณสมบัติ Azure active](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)directory</span><span class="sxs-lookup"><span data-stu-id="7347c-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="7347c-109">ที่ด้านล่างของหน้าให้คลิก**จัดการค่าเริ่มต้นด้านความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="7347c-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="7347c-110">คลิก **ใช่** เพื่อเปิดใช้งานค่าเริ่มต้นของความปลอดภัยหรือ **ไม่ใช่** เพื่อปิดใช้งานค่าเริ่มต้นด้านความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="7347c-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
