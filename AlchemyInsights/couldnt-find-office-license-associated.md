---
title: การแก้ไขแอป Microsoft ๓๖๕ไม่สามารถค้นหาข้อความที่เกี่ยวข้องกับสิทธิ์การใช้งาน office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747714"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="20865-102">การแก้ไขข้อความ Microsoft ๓๖๕ apps "ไม่พบสิทธิ์การใช้งาน office ที่เกี่ยวข้อง"</span><span class="sxs-lookup"><span data-stu-id="20865-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="20865-103">ถ้าคุณได้รับข้อความนี้ให้ลองทำดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="20865-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="20865-104">ตรวจสอบไฟร์วอลล์ซอฟต์แวร์ป้องกันไวรัสและการตั้งค่าพร็อกซีของคุณเพื่อยืนยันว่าพวกเขาไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="20865-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="20865-105">ให้ดู[ที่ url และช่วงที่อยู่ IP ของ Microsoft ๓๖๕](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="20865-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="20865-106">เอาออกและ [กำหนดสิทธิ์การใช้งาน Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ใหม่สำหรับผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="20865-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="20865-107">เปิดแอป Office และ [ลงชื่อออกจาก](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) บัญชีผู้ใช้ใดๆที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="20865-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="20865-108">ไปที่การตั้งค่า Windows >**บัญชี**ผู้  >  ใช้**อีเมลของ**บัญชีผู้ใช้ & และเอาบัญชีผู้ใช้ที่ทำงานทั้งหมดออกยกเว้นบัญชีที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="20865-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="20865-109">ไปที่การตั้งค่า**Accounts**Windows > การ  >  **เข้าถึงบัญชีผู้ใช้ที่ทำงานหรือโรงเรียน**และยกเลิกการเชื่อมต่อบัญชีที่ทำงานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="20865-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="20865-110">ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่</span><span class="sxs-lookup"><span data-stu-id="20865-110">Reset the Office activation state.</span></span> <span data-ttu-id="20865-111">[เรียนรู้วิธี](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)การ</span><span class="sxs-lookup"><span data-stu-id="20865-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="20865-112">[ลงชื่อเข้า](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) ใช้โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="20865-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="20865-113">สำหรับโซลูชันการแก้ไขปัญหาเพิ่มเติมให้ดู[ที่ข้อผิดพลาดในการเปิดใช้งานผลิตภัณฑ์และการเปิดใช้งานใน Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="20865-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>