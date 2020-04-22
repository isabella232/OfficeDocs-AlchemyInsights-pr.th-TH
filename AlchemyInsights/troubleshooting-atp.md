---
title: การแก้ไขปัญหาการป้องกันภัยคุกคามขั้นสูงของ Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: c90c8e9cb23cba93883cc1148fcbca77c9e92408
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732421"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="786a8-102">การแก้ไขปัญหาการป้องกันภัยคุกคามขั้นสูงของ Office 365</span><span class="sxs-lookup"><span data-stu-id="786a8-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="786a8-103">คุณสังเกตเห็นความล่าช้าในการส่งข้อความ?</span><span class="sxs-lookup"><span data-stu-id="786a8-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="786a8-104">ใช้ตัวเลือก[การจัดส่งแบบไดนามิก](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing)ในนโยบายสิ่งที่แนบที่ปลอดภัยของ ATP</span><span class="sxs-lookup"><span data-stu-id="786a8-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="786a8-105">วิธีนี้จะช่วยหลีกเลี่ยงความล่าช้าของข้อความในขณะที่ปกป้องผู้รับจากไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="786a8-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="786a8-106">คุณต้องการรายงานค่าบวกที่ผิดพลาดหรือเชิงลบที่ผิดพลาดต่อ Microsoft หรือไม่</span><span class="sxs-lookup"><span data-stu-id="786a8-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="786a8-107">ใช้[การเชื่อมโยง](https://www.microsoft.com/wdsi/filesubmission/)นี้เพื่อส่งไฟล์สําหรับการวิเคราะห์</span><span class="sxs-lookup"><span data-stu-id="786a8-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="786a8-108">คุณทราบหรือไม่ว่าคุณสามารถเปิดใช้งานการป้องกัน Safe Links สําหรับอีเมลภายในที่ส่งระหว่างผู้รับภายในองค์กรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="786a8-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="786a8-109">ทําตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="786a8-109">Follow these steps:</span></span>

  1. <span data-ttu-id="786a8-110">ไปที่[https://protection.office.com](https://protection.office.com)และลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลระบบส่วนกลางหรือบัญชีผู้ดูแลความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="786a8-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="786a8-111">ในบานหน้าต่างนําทางด้านซ้ายภายใต้**การจัดการภัยคุกคาม**ให้เลือก**ลิงก์ที่ปลอดภัย\*\*\*\*ของนโยบาย**\></span><span class="sxs-lookup"><span data-stu-id="786a8-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="786a8-112">ในส่วน**นโยบายที่ใช้กับทั้งองค์กร**ให้เลือกนโยบายและคลิก**แก้ไข**</span><span class="sxs-lookup"><span data-stu-id="786a8-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="786a8-113">ภายใต้**การตั้งค่า**ให้เปิดใช้งาน**ใช้ลิงก์ที่ปลอดภัยกับข้อความที่ส่งภายในองค์กร**</span><span class="sxs-lookup"><span data-stu-id="786a8-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
