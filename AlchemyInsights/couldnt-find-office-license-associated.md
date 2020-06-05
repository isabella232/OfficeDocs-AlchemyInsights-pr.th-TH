---
title: การแก้ไขแอป Microsoft 365 ไม่พบข้อความที่เกี่ยวข้องสิทธิ์การใช้งานสํานักงาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580460"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="d1eb2-102">การแก้ไขแอป Microsoft 365 "ไม่พบใบอนุญาตสํานักงานที่เกี่ยวข้อง"</span><span class="sxs-lookup"><span data-stu-id="d1eb2-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="d1eb2-103">หากคุณได้รับข้อความนี้ ให้ลองทําดังต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="d1eb2-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d1eb2-104">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าไฟร์วอลล์ไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d1eb2-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="d1eb2-105">ดู[Url 365 ของ Microsoft และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="d1eb2-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="d1eb2-106">เอาออก และ[กําหนดสิทธิ์การใช้งาน Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)สําหรับผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="d1eb2-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="d1eb2-107">เปิดแอป Office และ[ออกจากระบบ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)บัญชีผู้ใช้ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="d1eb2-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="d1eb2-108">ไปที่ การตั้งค่า Windows >**Accounts**  >  **บัญชีอีเมล & บัญชี**และลบบัญชีงานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="d1eb2-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="d1eb2-109">ไปที่ การตั้งค่า Windows >**งานของบัญชีผู้ใช้**  >  **Access หรือโรงเรียน**และยกเลิกการเชื่อมต่อบัญชีงานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="d1eb2-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="d1eb2-110">ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่</span><span class="sxs-lookup"><span data-stu-id="d1eb2-110">Reset the Office activation state.</span></span> <span data-ttu-id="d1eb2-111">[เรียนรู้วิธี](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="d1eb2-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="d1eb2-112">[เข้าสู่ระบบ](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="d1eb2-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="d1eb2-113">สําหรับการแก้ไขปัญหาเพิ่มเติม ให้ดูที่[ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งานและข้อผิดพลาดในการเปิดใช้งานใน Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="d1eb2-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>