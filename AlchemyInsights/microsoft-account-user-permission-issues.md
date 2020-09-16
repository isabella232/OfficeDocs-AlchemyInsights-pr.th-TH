---
title: แก้ไขปัญหา-ผู้ใช้ที่ไม่พบในไดเรกทอรี
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725426"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="cb8c6-102">แก้ไขปัญหา-ผู้ใช้ที่ไม่พบในไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="cb8c6-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="cb8c6-103">ถ้าผู้ใช้ได้รับข้อความแสดงข้อผิดพลาด "ไม่พบผู้ใช้" ในไดเรกทอรีโปรดลองอีกครั้งว่าชนิดของปัญหาคือผู้ใช้ที่ไม่ได้อยู่ในไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="cb8c6-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="cb8c6-104">ขั้นตอนต่อไปนี้สามารถทำให้เสร็จสมบูรณ์ได้เพื่อแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="cb8c6-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="cb8c6-105">ตรวจสอบให้แน่ใจว่าบัญชีผู้ใช้ที่ยอมรับคำเชิญทางอีเมลเป็นบัญชีผู้ใช้เดียวกันกับที่ใช้ในการลงชื่อเข้าใช้ในภายหลัง</span><span class="sxs-lookup"><span data-stu-id="cb8c6-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="cb8c6-106">ตรวจสอบให้แน่ใจว่าผู้ใช้กำลังใช้บัญชีผู้ใช้เดียวกันเพื่อยอมรับการเชิญและลงชื่อเข้าใช้ไซต์</span><span class="sxs-lookup"><span data-stu-id="cb8c6-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="cb8c6-107">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่วิธีการจัดการนามแฝงสำหรับบัญชี microsoft ของคุณ </a> เพื่อจัดการการเข้าสู่ระบบ microsoft ๓๖๕](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)</span><span class="sxs-lookup"><span data-stu-id="cb8c6-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="cb8c6-108">เรียกดูไซต์แต่ละไซต์ที่ผู้ใช้ได้รับข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="cb8c6-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="cb8c6-109">เพิ่ม "/_layouts/15/people.aspx/membershipgroupid = 0" (ภายในเครื่องหมายอัญประกาศคู่) จนถึงจุดสิ้นสุดของ URL ของไซต์</span><span class="sxs-lookup"><span data-stu-id="cb8c6-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="cb8c6-110">ตัวอย่าง: https://< "contoso" > sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0</span><span class="sxs-lookup"><span data-stu-id="cb8c6-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="cb8c6-111">เลือกผู้ใช้จากรายการ</span><span class="sxs-lookup"><span data-stu-id="cb8c6-111">Select the user from the list.</span></span>

- <span data-ttu-id="cb8c6-112">คลิก **เอาสิทธิ์ของผู้ใช้ออก** จาก Ribbon</span><span class="sxs-lookup"><span data-stu-id="cb8c6-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="cb8c6-113">เพิ่มกลับผู้ใช้และส่งการเชิญไปยังผู้ใช้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="cb8c6-113">Add back the User and Resend the invite to the user.</span></span>

