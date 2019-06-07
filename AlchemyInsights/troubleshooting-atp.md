---
title: การแก้ไขปัญหาการป้องกันการคุกคามขั้นสูง 365 Office
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: b4358fb55a1145833510c6063b520d822f2d1eaf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765493"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="ebc78-102">การแก้ไขปัญหาการป้องกันการคุกคามขั้นสูง 365 Office</span><span class="sxs-lookup"><span data-stu-id="ebc78-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="ebc78-103">คุณพบความล่าช้าในการส่งข้อความได้อย่างไร</span><span class="sxs-lookup"><span data-stu-id="ebc78-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="ebc78-104">ใช้ตัวเลือกการ[จัดส่งแบบไดนามิก](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing)ในนโยบาย ATP เซฟสิ่งที่แนบมาของคุณ</span><span class="sxs-lookup"><span data-stu-id="ebc78-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="ebc78-105">ซึ่งจะช่วยหลีกเลี่ยงความล่าช้าของข้อความในขณะที่ผู้รับการปกป้องจากแฟ้มที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="ebc78-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="ebc78-106">คุณต้องการรายงานการทำงานผิดพลาดเท็จหรือ false ค่าลบไปยัง Microsoft ได้อย่างไร</span><span class="sxs-lookup"><span data-stu-id="ebc78-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="ebc78-107">ใช้[การเชื่อมโยง](https://www.microsoft.com/wdsi/filesubmission/)นี้เพื่อส่งไฟล์สำหรับการวิเคราะห์</span><span class="sxs-lookup"><span data-stu-id="ebc78-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="ebc78-108">คุณทราบว่า คุณสามารถเปิดใช้งานการป้องกันเชื่อมโยงปลอดภัยสำหรับอีเมลภายในที่ส่งระหว่างผู้รับภายในองค์กรของคุณได้อย่างไร</span><span class="sxs-lookup"><span data-stu-id="ebc78-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="ebc78-109">ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="ebc78-109">Follow these steps:</span></span>

  1. <span data-ttu-id="ebc78-110">ไปที่[https://protection.office.com](https://protection.office.com)และเข้าสู่ระบบ ด้วยการดูแลส่วนกลางหรือบัญชีผู้ดูแลความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="ebc78-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="ebc78-111">ในบานหน้าต่างนำทางด้านซ้ายภายใต้การ**บริหารความเสี่ยง**เลือก**นโยบาย** \> **การเชื่อมโยงที่ปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="ebc78-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="ebc78-112">ในส่วนของ**นโยบายที่นำไปใช้กับทั้งองค์กร**นโยบายเลือก และคลิก**แก้ไข**</span><span class="sxs-lookup"><span data-stu-id="ebc78-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="ebc78-113">ภายใต้การ**ตั้งค่า**เปิดใช้งานการ**เชื่อมโยงเซฟนำไปใช้กับข้อความที่ส่งภายในองค์กร**</span><span class="sxs-lookup"><span data-stu-id="ebc78-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
