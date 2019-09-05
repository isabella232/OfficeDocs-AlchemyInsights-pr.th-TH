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
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754211"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="1501c-102">แก้ไขปัญหา-ไม่พบผู้ใช้ในไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="1501c-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="1501c-103">ถ้าผู้ใช้ได้รับข้อความข้อผิดพลาด "ผู้ใช้ไม่พบ" ในไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="1501c-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="1501c-104">โปรดลองอีกครั้งที่ชนิดของปัญหาเป็นผู้ใช้ไม่อยู่ในไดเรกทอรี</span><span class="sxs-lookup"><span data-stu-id="1501c-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="1501c-105">ขั้นตอนต่อไปนี้สามารถทำให้เสร็จสมบูรณ์เพื่อแก้ไขปัญหา</span><span class="sxs-lookup"><span data-stu-id="1501c-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="1501c-106">ตรวจสอบให้แน่ใจว่าบัญชีที่ยอมรับการเชิญทางเมลเป็นบัญชีเดียวกันกับที่ใช้ในการเข้าสู่ระบบในภายหลัง</span><span class="sxs-lookup"><span data-stu-id="1501c-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="1501c-107">ตรวจสอบให้แน่ใจว่าผู้ใช้ใช้บัญชีเดียวกันเพื่อยอมรับการเชิญและลงชื่อเข้าใช้เว็บไซต์</span><span class="sxs-lookup"><span data-stu-id="1501c-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="1501c-108">สำหรับข้อมูลเพิ่มเติมให้ดู[วิธีการจัดการนามแฝงสำหรับบัญชี</a> Microsoft ของคุณเพื่อจัดการ Office ๓๖๕เข้าสู่ระบบ](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)</span><span class="sxs-lookup"><span data-stu-id="1501c-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="1501c-109">เรียกดูไปยังแต่ละไซต์ที่ผู้ใช้ได้รับข้อผิดพลาด</span><span class="sxs-lookup"><span data-stu-id="1501c-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="1501c-110">เพิ่ม "/_layouts/15/people.aspx/membershipgroupid = 0" (ภายในอัญประกาศคู่) ไปยังจุดสิ้นสุดของ URL ของไซต์</span><span class="sxs-lookup"><span data-stu-id="1501c-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="1501c-111">ตัวอย่าง: https://_lt_ "contoso">/_ เค้าโครง/15/คน. aspx/membershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="1501c-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="1501c-112">เลือกผู้ใช้จากรายการ</span><span class="sxs-lookup"><span data-stu-id="1501c-112">Select the user from the list.</span></span>

- <span data-ttu-id="1501c-113">คลิ**กเอาออกสิทธิ์ของผู้ใช้**จาก Ribbon</span><span class="sxs-lookup"><span data-stu-id="1501c-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="1501c-114">เพิ่มผู้ใช้และส่งการเชิญไปยังผู้ใช้อีกครั้ง</span><span class="sxs-lookup"><span data-stu-id="1501c-114">Add back the User and Resend the invite to the user.</span></span>

