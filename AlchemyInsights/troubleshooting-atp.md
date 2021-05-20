---
title: การแก้ไขปัญหา Microsoft Defender Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545287"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="562bd-102">การแก้ไขปัญหา Microsoft Defender Office 365</span><span class="sxs-lookup"><span data-stu-id="562bd-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="562bd-103">**คุณสังเกตเห็นความล่าช้าในการส่งข้อความหรือไม่**</span><span class="sxs-lookup"><span data-stu-id="562bd-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="562bd-104">ใช้ตัวเลือก[การจัดส่งแบบไดนามิก](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing)ใน Microsoft Defender ของคุณOffice 365นโยบายสิ่งที่แนบมาที่ปลอดภัยของคุณ</span><span class="sxs-lookup"><span data-stu-id="562bd-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="562bd-105">ซึ่งจะช่วยหลีกเลี่ยงความล่าช้าของข้อความในขณะที่ป้องกันผู้รับจากไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="562bd-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="562bd-106">**คุณต้องการรายงานผลลัพธ์ที่ผิดหรือเป็นลบที่ผิดไปยัง Microsoft หรือไม่**</span><span class="sxs-lookup"><span data-stu-id="562bd-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="562bd-107">ใช้[Submissions Explorer](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="562bd-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="562bd-108">-\*\* คุณทราบหรือไม่ว่าคุณสามารถเปิดใช้งานการป้องกันลิงก์ที่ปลอดภัยให้กับอีเมลภายในที่ส่งระหว่างผู้รับภายในองค์กรของคุณได้\*\* ให้ปฏิบัติตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="562bd-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="562bd-109">ไปที่ [https://protection.office.com](https://protection.office.com) และลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลระบบส่วนกลางหรือผู้ดูแลระบบความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="562bd-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="562bd-110">ในบานหน้าต่างนําทางด้านซ้าย ภายใต้ **การจัดการภัยคุกคาม** ให้เลือก **ลิงก์** \> **นโยบาย** ที่ปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="562bd-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="562bd-111">ในส่วน **นโยบายที่มีผลบังคับใช้กับทั้ง** องค์กร ให้เลือกนโยบาย **แล้วคลิก** แก้ไข</span><span class="sxs-lookup"><span data-stu-id="562bd-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="562bd-112">ภายใต้ **การตั้งค่า** ให้เปิดใช้งาน **ใช้ลิงก์ที่ปลอดภัยกับข้อความที่ส่งภายใน** องค์กร</span><span class="sxs-lookup"><span data-stu-id="562bd-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
