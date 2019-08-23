---
title: แก้ไขปัญหา - ไม่พบในไดเรกทอรีของผู้ใช้
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544882"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="d24ae-102">แก้ไขปัญหา - ไม่พบในไดเรกทอรีของผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d24ae-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="d24ae-103">ถ้าผู้ใช้ได้รับข้อผิดพลาดข้อความ "ไม่พบผู้ใช้" ในไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="d24ae-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="d24ae-104">โปรดลองอีกครั้ง ที่ชนิดการตัดสินค้าจากคลังที่ผู้ใช้ไม่มีไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="d24ae-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="d24ae-105">ขั้นตอนต่อไปนี้สามารถให้สมบูรณ์เพื่อแก้ปัญหา</span><span class="sxs-lookup"><span data-stu-id="d24ae-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="d24ae-106">ให้แน่ใจว่าบัญชีที่ยอมรับการเชิญทางอีเมลเป็นบัญชีเดียวกับที่ใช้เข้าสู่ระบบในภายหลัง</span><span class="sxs-lookup"><span data-stu-id="d24ae-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="d24ae-107">ตรวจสอบให้แน่ใจว่า ผู้ใช้ที่กำลังใช้บัญชีเดียวกันเพื่อยอมรับการเชิญ และเซ็นชื่อลงในไซต์</span><span class="sxs-lookup"><span data-stu-id="d24ae-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="d24ae-108">สำหรับข้อมูลเพิ่มเติม ดู[วิธีการจัดการนามแฝงสำหรับบัญชีของคุณ Microsoft</a>การจัดการการเข้าสู่ระบบ Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)</span><span class="sxs-lookup"><span data-stu-id="d24ae-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="d24ae-109">เรียกดูไซต์แต่ละผู้ใช้ได้รับข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="d24ae-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="d24ae-110">เพิ่ม " / _layouts/15/people.aspx/membershipgroupid=0 " (ภายในอัญประกาศ) ลงในส่วนท้ายของ URL ของไซต์</span><span class="sxs-lookup"><span data-stu-id="d24ae-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="d24ae-111">ตัวอย่าง: _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 https://_lT</span><span class="sxs-lookup"><span data-stu-id="d24ae-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="d24ae-112">เลือกผู้ใช้จากรายการ</span><span class="sxs-lookup"><span data-stu-id="d24ae-112">Select the user from the list.</span></span>

- <span data-ttu-id="d24ae-113">คลิก**เอาออกสิทธิ์ของผู้ใช้**จาก Ribbon</span><span class="sxs-lookup"><span data-stu-id="d24ae-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="d24ae-114">เพิ่มผู้ใช้กลับ และส่งการเชิญไปยังผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="d24ae-114">Add back the User and Resend the invite to the user.</span></span>

