---
title: การรับรองความถูกต้องแบบหลายปัจจัยที่ไม่คาดคิด
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 48303d5b408cbdb243ec45dc4c80ac9a83f273a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689541"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="fa1f6-102">การรับรองความถูกต้องแบบหลายปัจจัยที่ไม่คาดคิด</span><span class="sxs-lookup"><span data-stu-id="fa1f6-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="fa1f6-103">ถ้าผู้เช่าของคุณถูกสร้างขึ้นหลังจากวันที่21ตุลาคม๒๐๑๙และคุณจะได้รับพร้อมท์สำหรับ MFA โดยไม่คาดคิดคุณอาจมี [ค่าเริ่มต้นของความปลอดภัย](https://aka.ms/securitydefaults) ที่เปิดใช้งานในผู้เช่าของคุณ</span><span class="sxs-lookup"><span data-stu-id="fa1f6-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="fa1f6-104">เมื่อต้องการจัดการค่าเริ่มต้นของความปลอดภัย:</span><span class="sxs-lookup"><span data-stu-id="fa1f6-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="fa1f6-105">ลงชื่อเข้าใช้ [ศูนย์การจัดการ](https://go.microsoft.com/fwlink/p/?linkid=834822) ด้วยข้อมูลประจำตัวของผู้ดูแลระบบส่วนกลางของคุณ</span><span class="sxs-lookup"><span data-stu-id="fa1f6-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="fa1f6-106">ไปยัง [คุณสมบัติ Azure active](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)directory</span><span class="sxs-lookup"><span data-stu-id="fa1f6-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="fa1f6-107">ที่ด้านล่างของหน้าให้คลิก**จัดการค่าเริ่มต้นด้านความปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="fa1f6-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="fa1f6-108">คลิก **ใช่** เพื่อเปิดใช้งานค่าเริ่มต้นของความปลอดภัยและ **ไม่** ต้องปิดใช้งานค่าเริ่มต้นของความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="fa1f6-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
