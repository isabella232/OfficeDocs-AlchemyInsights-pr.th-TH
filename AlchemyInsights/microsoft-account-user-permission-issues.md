---
title: แก้ไขปัญหา-ไม่พบผู้ใช้ในไดเรกทอรี
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768820"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="f82a5-102">แก้ไขปัญหา-ไม่พบผู้ใช้ในไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="f82a5-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="f82a5-103">ถ้าผู้ใช้ได้รับข้อความข้อผิดพลาด "ผู้ใช้ไม่พบ" ในไดเรกทอรีโปรดลองอีกครั้งที่ชนิดของปัญหาเป็นผู้ใช้ไม่ได้อยู่ในไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="f82a5-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="f82a5-104">ขั้นตอนต่อไปนี้สามารถทำให้เสร็จสมบูรณ์เพื่อแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="f82a5-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="f82a5-105">ตรวจสอบให้แน่ใจว่าบัญชีที่ยอมรับการเชิญทางเมลเป็นบัญชีเดียวกันกับที่ใช้ในการเข้าสู่ระบบในภายหลัง</span><span class="sxs-lookup"><span data-stu-id="f82a5-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="f82a5-106">ตรวจสอบให้แน่ใจว่าผู้ใช้ใช้บัญชีเดียวกันเพื่อยอมรับการเชิญและลงชื่อเข้าใช้เว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="f82a5-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="f82a5-107">สำหรับข้อมูลเพิ่มเติมให้ดู[วิธีการจัดการนามแฝงสำหรับบัญชี</a> Microsoft ของคุณเพื่อจัดการ Office ๓๖๕เข้าสู่ระบบ](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)</span><span class="sxs-lookup"><span data-stu-id="f82a5-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="f82a5-108">เรียกดูไปยังแต่ละไซต์ที่ผู้ใช้ได้รับข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="f82a5-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="f82a5-109">เพิ่ม "/_layouts/15/people.aspx/membershipgroupid = 0" (ภายในอัญประกาศคู่) ไปยังจุดสิ้นสุดของ URL ของไซต์</span><span class="sxs-lookup"><span data-stu-id="f82a5-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="f82a5-110">ตัวอย่าง: https://< "contoso" > sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0</span><span class="sxs-lookup"><span data-stu-id="f82a5-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="f82a5-111">เลือกผู้ใช้จากรายการ</span><span class="sxs-lookup"><span data-stu-id="f82a5-111">Select the user from the list.</span></span>

- <span data-ttu-id="f82a5-112">คลิ**กเอาออกสิทธิ์ของผู้ใช้**จาก Ribbon</span><span class="sxs-lookup"><span data-stu-id="f82a5-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="f82a5-113">เพิ่มผู้ใช้และส่งการเชิญไปยังผู้ใช้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="f82a5-113">Add back the User and Resend the invite to the user.</span></span>

