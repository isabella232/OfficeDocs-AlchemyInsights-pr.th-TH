---
title: นโยบายการเข้าถึงแบบมีเงื่อนไข
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 569507318b499cdbcf2a1cd75e84046953f62212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706076"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="26669-102">นโยบายการเข้าถึงแบบมีเงื่อนไข</span><span class="sxs-lookup"><span data-stu-id="26669-102">Conditional Access policies</span></span>

<span data-ttu-id="26669-103">การเข้าถึงแบบมีเงื่อนไขคือความสามารถของ Azure AD ที่ช่วยให้คุณสามารถบังคับใช้การควบคุมการเข้าถึงแอปในสภาพแวดล้อมของคุณ ทั้งหมดขึ้นอยู่กับเงื่อนไขเฉพาะและจัดการจากตําแหน่งที่ตั้งส่วนกลาง</span><span class="sxs-lookup"><span data-stu-id="26669-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="26669-104">เรียนรู้เพิ่มเติมเกี่ยวกับ[การเข้าถึงแบบมีเงื่อนไขโฆษณา Azure](https://docs.microsoft.com/azure/active-directory/conditional-access/)</span><span class="sxs-lookup"><span data-stu-id="26669-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="26669-105">**หมายเหตุ**: ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่ 21 ตุลาคม 2019 และคุณได้รับพร้อมท์สําหรับ MFA โดยไม่คาดคิด คุณอาจมี[ค่าเริ่มต้นการรักษาความปลอดภัย](https://aka.ms/securitydefaults)ที่เปิดใช้งานในผู้เช่าของคุณโดยไม่คาดคิด</span><span class="sxs-lookup"><span data-stu-id="26669-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="26669-106">**เมื่อต้องการจัดการค่าเริ่มต้นความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="26669-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="26669-107">ลงชื่อเข้าใช้[ศูนย์การจัดการ](https://go.microsoft.com/fwlink/p/?linkid=834822)ด้วยข้อมูลประจําตัวของผู้ดูแลระบบส่วนกลางของคุณ</span><span class="sxs-lookup"><span data-stu-id="26669-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="26669-108">ไปที่[คุณสมบัติไดเรกทอรีที่ใช้งานอยู่ของ Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)</span><span class="sxs-lookup"><span data-stu-id="26669-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="26669-109">ที่ด้านล่างของหน้า ให้คลิก**จัดการค่าเริ่มต้นความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="26669-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="26669-110">คลิก**ใช่**เพื่อเปิดใช้งานค่าเริ่มต้นการรักษาความปลอดภัยหรือ**ไม่ใช่**เพื่อปิดใช้งานค่าเริ่มต้นการรักษาความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="26669-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
