---
title: การแก้ไขแอป Office ไม่พบข้อความที่เกี่ยวข้องเกี่ยวกับสิทธิ์การใช้งาน Office
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
ms.openlocfilehash: 565df0a05baa974a6cbac58ac6be8d78470dbc5d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715651"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="8226c-102">การแก้ไขข้อความ "ไม่พบสิทธิ์การใช้งาน Office ที่เกี่ยวข้อง"</span><span class="sxs-lookup"><span data-stu-id="8226c-102">Fixing the Office apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="8226c-103">ถ้าคุณได้รับข้อความนี้ ให้ลองทําดังต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="8226c-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="8226c-104">ตรวจสอบไฟร์วอลล์ ซอฟต์แวร์ป้องกันไวรัส และการตั้งค่าพร็อกซีเพื่อยืนยันว่าจะไม่บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Office</span><span class="sxs-lookup"><span data-stu-id="8226c-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="8226c-105">ดู[URL ของ Microsoft 365 และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="8226c-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="8226c-106">เอาออก และ[กําหนดสิทธิ์การใช้งาน Office](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users)สําหรับผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="8226c-106">Remove and [reassign the Office license](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="8226c-107">เปิดแอป Office และ[ลงชื่อออกจาก](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)บัญชีผู้ใช้ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="8226c-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="8226c-108">ไปที่ การตั้งค่า windows > > **บัญชีอีเมลบัญชี &** และเอาบัญชีการทํางานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ**Accounts**</span><span class="sxs-lookup"><span data-stu-id="8226c-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="8226c-109">ไปที่ การตั้งค่า Windows **>** > **ทํางานหรือโรงเรียนการเข้าถึง**และยกเลิกการเชื่อมต่อบัญชีที่ทํางานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="8226c-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="8226c-110">ตั้งค่าสถานะการเปิดใช้งาน Office ใหม่</span><span class="sxs-lookup"><span data-stu-id="8226c-110">Reset the Office activation state.</span></span> <span data-ttu-id="8226c-111">[เรียนรู้วิธี](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="8226c-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="8226c-112">[ลงชื่อเข้าใช้](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)โดยใช้บัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="8226c-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="8226c-113">สําหรับการแก้ไขปัญหาเพิ่มเติม ให้ดูที่[ผลิตภัณฑ์ที่ไม่มีสิทธิ์การใช้งานและข้อผิดพลาดในการเปิดใช้งานใน Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="8226c-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>