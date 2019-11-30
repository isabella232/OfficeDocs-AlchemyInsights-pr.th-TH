---
title: แก้ไขแอป Office ไม่พบข้อความที่เกี่ยวข้องกับสิทธิ์การใช้งาน office
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
ms.openlocfilehash: 1820cdb83a1adf36b4e7d0898ecdf8097eb6f0f3
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627937"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="7dd77-102">การแก้ไขแอป Office "ไม่พบข้อความใบอนุญาตของ office ที่เกี่ยวข้อง"</span><span class="sxs-lookup"><span data-stu-id="7dd77-102">Fixing the Office apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="7dd77-103">ถ้าคุณได้รับข้อความนี้ให้ลองทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="7dd77-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="7dd77-104">ตรวจสอบไฟร์วอลล์ซอฟต์แวร์ป้องกันไวรัสและการตั้งค่าพร็อกซีเพื่อยืนยันว่าพวกเขาไม่ได้บล็อกการเข้าถึงอินเทอร์เน็ตไปยังแอป Office</span><span class="sxs-lookup"><span data-stu-id="7dd77-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="7dd77-105">ดู[url ของ Office ๓๖๕และช่วงที่อยู่ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="7dd77-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="7dd77-106">เอาออกและ[มอบหมายใบอนุญาต Office](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users)สำหรับผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="7dd77-106">Remove and [reassign the Office license](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="7dd77-107">เปิดแอป Office แล้ว[ลงชื่อออก](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)จากบัญชีผู้ใช้ที่มีอยู่</span><span class="sxs-lookup"><span data-stu-id="7dd77-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="7dd77-108">ไปที่การตั้งค่า Windows >**บัญชี** > **& บัญชี**ของคุณและลบบัญชีงานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="7dd77-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="7dd77-109">ไปที่การตั้งค่า Windows >**บัญชี** > การ**เข้าถึงที่ทำงานหรือโรงเรียน**และยกเลิกการเชื่อมต่อบัญชีการทำงานทั้งหมดยกเว้นบัญชีที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="7dd77-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="7dd77-110">รีเซ็ตสถานะการเปิดใช้งาน Office</span><span class="sxs-lookup"><span data-stu-id="7dd77-110">Reset the Office activation state.</span></span> <span data-ttu-id="7dd77-111">[เรียนรู้วิธี](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)การ</span><span class="sxs-lookup"><span data-stu-id="7dd77-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="7dd77-112">[ลงชื่อเข้า](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9)ใช้ด้วยบัญชีผู้ใช้ที่ได้รับผลกระทบ</span><span class="sxs-lookup"><span data-stu-id="7dd77-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="7dd77-113">สำหรับโซลูชันการแก้ไขปัญหาเพิ่มเติมโปรดดูที่[ข้อผิดพลาดของผลิตภัณฑ์และการเปิดใช้งานใน Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="7dd77-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>