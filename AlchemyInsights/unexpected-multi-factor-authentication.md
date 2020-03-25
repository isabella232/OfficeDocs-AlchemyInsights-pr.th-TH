---
title: การรับรองความถูกต้องด้วยหลายปัจจัยที่ไม่คาดคิด
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946852"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="ae876-102">การรับรองความถูกต้องด้วยหลายปัจจัยที่ไม่คาดคิด</span><span class="sxs-lookup"><span data-stu-id="ae876-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="ae876-103">ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่ 21 ตุลาคม 2019 และคุณได้รับพร้อมท์สําหรับ MFA โดยไม่คาดคิด คุณอาจมี[ค่าเริ่มต้นการรักษาความปลอดภัย](http://aka.ms/securitydefaults)ที่เปิดใช้งานในผู้เช่าของคุณโดยไม่คาดคิด</span><span class="sxs-lookup"><span data-stu-id="ae876-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="ae876-104">เมื่อต้องการจัดการค่าเริ่มต้นความปลอดภัย:</span><span class="sxs-lookup"><span data-stu-id="ae876-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="ae876-105">ลงชื่อเข้าใช้[ศูนย์การจัดการ](https://go.microsoft.com/fwlink/p/?linkid=834822)ด้วยข้อมูลประจําตัวของผู้ดูแลระบบส่วนกลางของคุณ</span><span class="sxs-lookup"><span data-stu-id="ae876-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="ae876-106">ไปที่[คุณสมบัติไดเรกทอรีที่ใช้งานอยู่ของ Azure](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)</span><span class="sxs-lookup"><span data-stu-id="ae876-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="ae876-107">ที่ด้านล่างของหน้า ให้คลิก**จัดการค่าเริ่มต้นความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="ae876-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="ae876-108">คลิก**ใช่**เพื่อเปิดใช้งานค่าเริ่มต้นการรักษาความปลอดภัยและ**ไม่ใช่**เพื่อปิดใช้งานค่าเริ่มต้นการรักษาความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="ae876-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
