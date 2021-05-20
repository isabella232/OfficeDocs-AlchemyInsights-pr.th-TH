---
title: Teams Add-in for Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582089"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="59aef-102">Teams Add-in for Mac</span><span class="sxs-lookup"><span data-stu-id="59aef-102">Teams add-in for Mac</span></span>

<span data-ttu-id="59aef-103">เมื่อต้องการแก้ไขปัญหาเกี่ยวกับTeams Add-in for Mac ผู้ใช้ระบบปฏิบัติการ ให้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="59aef-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="59aef-104">**ขั้นตอนที่ 1:** ถ้าคุณมีไฮบริด Exchangeภายในองค์กร (2016 CU3 หรือใหม่กว่าที่กําหนดค่า) ให้ใช้เครื่องมือ Test-HMA.ps1 เพื่อยืนยันว่า การรับรองความถูกต้องสมัยใหม่แบบไฮบริดได้รับการกําหนดค่าอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="59aef-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="59aef-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span><span class="sxs-lookup"><span data-stu-id="59aef-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="59aef-106">**หมายเหตุ** ใช้รูปแบบที่อยู่ UPN (ตัวอย่างเช่น username@contoso.com [)](mailto:username@contoso.com)ไม่ใช่ โดเมน\ชื่อผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="59aef-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="59aef-107">วิธีนี้แม้กับผู้ใช้ที่มีExchange Onlineกล่องจดหมายของคุณ</span><span class="sxs-lookup"><span data-stu-id="59aef-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="59aef-108">**ขั้นตอนที่ 2:** ให้ผู้ใช้ไปที่ บัญชี  >  **เครื่องมือ**... ใน Outlook for Mac บัญชี แล้วค้นหาและเลือกบัญชี</span><span class="sxs-lookup"><span data-stu-id="59aef-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="59aef-109">ยืนยันว่าชื่อผู้ใช้ที่แสดงรายการอยู่ในรูปแบบ UPN (ตัวอย่างเช่น [username@contoso.com](mailto:username@contoso.com))</span><span class="sxs-lookup"><span data-stu-id="59aef-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="59aef-110">**ขั้นตอนที่ 3:** ยืนยันว่าผู้ใช้เป็นผู้ใช้ที่มีMicrosoft Teamsสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="59aef-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="59aef-111">ผู้ใช้ต้องใช้การสมัครใช้งาน Office 365 for Mac ผลิตภัณฑ์เวอร์ชัน 16.24 หรือใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="59aef-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>