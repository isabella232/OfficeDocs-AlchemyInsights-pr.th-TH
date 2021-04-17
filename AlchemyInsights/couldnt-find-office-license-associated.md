---
title: การแก้ไขแอป Microsoft 365 ไม่พบข้อความที่เกี่ยวข้องกับสิทธิ์การใช้งาน Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816507"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="62ea2-102">การแก้ไขข้อความ "ไม่พบสิทธิ์การใช้งาน Office ที่เชื่อมโยงกัน" ของแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="62ea2-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="62ea2-103">ถ้าคุณได้รับข้อความนี้ ให้ลองวิธีต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="62ea2-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="62ea2-104">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="62ea2-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="62ea2-105">ดู[URL และช่วงที่อยู่ IP ของ Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="62ea2-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="62ea2-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span><span class="sxs-lookup"><span data-stu-id="62ea2-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="62ea2-107">เปิดแอป Office [แล้วลงชื่อ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) ออกจากบัญชีผู้ใช้ใดๆ ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="62ea2-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="62ea2-108">ไปที่ การตั้งค่า Windows >  >  **บัญชีอีเมล& บัญชี** และเอาบัญชีที่ได้ผลทั้งหมดออก ยกเว้นบัญชีที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="62ea2-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="62ea2-109">ไปที่ การตั้งค่า ของ Windows >  >  **การเข้าถึงบัญชีที่โรงเรียน** หรือที่โรงเรียน และยกเลิกการเชื่อมต่อบัญชีที่งานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="62ea2-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="62ea2-110">รีเซ็ตสถานะการเปิดใช้งาน Office</span><span class="sxs-lookup"><span data-stu-id="62ea2-110">Reset the Office activation state.</span></span> <span data-ttu-id="62ea2-111">[เรียนรู้วิธีการ](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="62ea2-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="62ea2-112">[ลงชื่อเข้าใช้](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) ด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="62ea2-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="62ea2-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="62ea2-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>