---
title: Add-in ของทีมสำหรับ Mac
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
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670347"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="99d37-102">Add-in ของทีมสำหรับ Mac</span><span class="sxs-lookup"><span data-stu-id="99d37-102">Teams add-in for Mac</span></span>

<span data-ttu-id="99d37-103">เมื่อต้องการแก้ไขปัญหาสำหรับผู้ใช้ระบบปฏิบัติการของระบบปฏิบัติการของ Mac ที่ขาดหายไปให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="99d37-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="99d37-104">**ขั้นตอนที่ 1:** ถ้าคุณมี Exchange แบบไฮบริดในองค์กร (๒๐๑๖ CU3 หรือใหม่กว่าที่จำเป็น) ให้ใช้เครื่องมือ Test-HMA.ps1 เพื่อยืนยันว่าการรับรองความถูกต้องแบบไฮบริดที่ทันสมัยถูกกำหนดค่าอย่างถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="99d37-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="99d37-105">สำหรับข้อมูลเพิ่มเติมให้ดูที่การ[ตรวจสอบการตั้งค่าการรับรองความถูกต้องแบบไฮบริดที่ทันสมัยสำหรับ Outlook สำหรับ iOS และ Android](https://aka.ms/AA980zq)</span><span class="sxs-lookup"><span data-stu-id="99d37-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="99d37-106">**หมายเหตุ:** ใช้รูปแบบที่อยู่ UPN (ตัวอย่างเช่น [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span><span class="sxs-lookup"><span data-stu-id="99d37-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="99d37-107">ให้ทำสิ่งนี้แม้แต่สำหรับผู้ใช้ที่มีกล่องจดหมาย Exchange Online</span><span class="sxs-lookup"><span data-stu-id="99d37-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="99d37-108">**ขั้นตอนที่ 2:** มีผู้ใช้ไปที่**บัญชีเครื่องมือ**  >  **Accounts**... ใน Outlook for Mac และค้นหาและเลือกบัญชีผู้ใช้</span><span class="sxs-lookup"><span data-stu-id="99d37-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="99d37-109">ยืนยันชื่อผู้ใช้ที่แสดงอยู่ในรูปแบบ UPN (ตัวอย่างเช่น [username@contoso.com](mailto:username@contoso.com))</span><span class="sxs-lookup"><span data-stu-id="99d37-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="99d37-110">**ขั้นตอนที่ 3:** ยืนยันผู้ใช้เป็นผู้ใช้ Microsoft team ที่ได้รับสิทธิ์การใช้งาน</span><span class="sxs-lookup"><span data-stu-id="99d37-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="99d37-111">ผู้ใช้ต้องใช้การสมัครใช้งาน Office ๓๖๕ for Mac เวอร์ชันผลิตภัณฑ์๑๖.๒๔หรือเวอร์ชันที่ใหม่กว่า</span><span class="sxs-lookup"><span data-stu-id="99d37-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>