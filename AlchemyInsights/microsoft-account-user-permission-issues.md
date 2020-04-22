---
title: แก้ไขปัญหา - ไม่พบผู้ใช้ในไดเรกทอรี
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702757"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="06787-102">แก้ไขปัญหา - ไม่พบผู้ใช้ในไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="06787-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="06787-103">หากผู้ใช้ได้รับข้อความแสดงข้อผิดพลาด "ไม่พบผู้ใช้" ในไดเรกทอรี โปรดลองอีกครั้งที่ประเภทปัญหาคือ ผู้ใช้ไม่ได้อยู่ในไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="06787-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="06787-104">ขั้นตอนต่อไปนี้สามารถเสร็จสมบูรณ์เพื่อแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="06787-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="06787-105">ตรวจสอบให้แน่ใจว่าบัญชีที่ยอมรับคําเชิญทางอีเมลเป็นบัญชีเดียวกับที่ใช้ในการลงชื่อเข้าใช้ในภายหลัง</span><span class="sxs-lookup"><span data-stu-id="06787-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="06787-106">ตรวจสอบว่าผู้ใช้ใช้บัญชีเดียวกันเพื่อยอมรับคําเชิญและลงชื่อเข้าใช้ไซต์</span><span class="sxs-lookup"><span data-stu-id="06787-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="06787-107">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[วิธีจัดการนามแฝงสําหรับบัญชี</a>Microsoft ของคุณเพื่อจัดการการเข้าสู่ระบบ Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)</span><span class="sxs-lookup"><span data-stu-id="06787-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="06787-108">เรียกดูแต่ละไซต์ซึ่งผู้ใช้ได้รับข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="06787-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="06787-109">เพิ่ม "/_layouts/15/people.aspx/membershipgroupid=0" (ภายในเครื่องหมายอัญประกาศคู่) ไปยังส่วนท้ายของ URL ของไซต์</span><span class="sxs-lookup"><span data-stu-id="06787-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="06787-110">ตัวอย่าง: https://<"contoso">.sharepoint.com/_layouts 15/people.aspx/สมาชิกกลุ่มId =0</span><span class="sxs-lookup"><span data-stu-id="06787-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="06787-111">เลือกผู้ใช้จากรายการ</span><span class="sxs-lookup"><span data-stu-id="06787-111">Select the user from the list.</span></span>

- <span data-ttu-id="06787-112">คลิก**เอาสิทธิ์ของผู้ใช้**ออกจาก Ribbon</span><span class="sxs-lookup"><span data-stu-id="06787-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="06787-113">เพิ่มกลับผู้ใช้และส่งคําเชิญไปยังผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="06787-113">Add back the User and Resend the invite to the user.</span></span>

