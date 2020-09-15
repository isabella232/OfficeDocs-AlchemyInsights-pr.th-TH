---
title: การแก้ไขปัญหาการป้องกันการคุกคามขั้นสูงของ Office ๓๖๕
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
ms.openlocfilehash: 5a13653ba08d8c6b822354ff70f6d276d31cd816
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658933"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="968c9-102">การแก้ไขปัญหาการป้องกันการคุกคามขั้นสูงของ Office ๓๖๕</span><span class="sxs-lookup"><span data-stu-id="968c9-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="968c9-103">คุณสังเกตเห็นความล่าช้าในการนำส่งข้อความหรือไม่</span><span class="sxs-lookup"><span data-stu-id="968c9-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="968c9-104">ใช้ตัวเลือกการนำ [ส่งแบบไดนามิก](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) ในนโยบายสิ่งที่แนบมาของ ATP Safe ของคุณ</span><span class="sxs-lookup"><span data-stu-id="968c9-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="968c9-105">การทำเช่นนี้จะช่วยหลีกเลี่ยงความล่าช้าของข้อความในขณะที่ปกป้องผู้รับจากไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="968c9-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="968c9-106">คุณต้องการรายงาน false บวกหรือค่าลบ false ไปยังไมโครซอฟท์หรือไม่</span><span class="sxs-lookup"><span data-stu-id="968c9-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="968c9-107">ใช้ [ลิงก์](https://www.microsoft.com/wdsi/filesubmission/) นี้เพื่อส่งไฟล์สำหรับการวิเคราะห์</span><span class="sxs-lookup"><span data-stu-id="968c9-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="968c9-108">คุณทราบหรือไม่ว่าคุณสามารถเปิดใช้งานการป้องกันลิงก์ที่ปลอดภัยสำหรับอีเมลภายในที่ส่งระหว่างผู้รับภายในองค์กรของคุณได้</span><span class="sxs-lookup"><span data-stu-id="968c9-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="968c9-109">ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="968c9-109">Follow these steps:</span></span>

  1. <span data-ttu-id="968c9-110">ไปที่ [https://protection.office.com](https://protection.office.com) แล้วลงชื่อเข้าใช้ด้วยบัญชีผู้ดูแลระบบส่วนกลางหรือบัญชีผู้ดูแลระบบความปลอดภัย</span><span class="sxs-lookup"><span data-stu-id="968c9-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="968c9-111">ในบานหน้าต่างนำทางด้านซ้ายภายใต้**การจัดการภัยคุกคาม**ให้เลือก**Policy** \> **ลิงก์ที่ปลอดภัย**ตามนโยบาย</span><span class="sxs-lookup"><span data-stu-id="968c9-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="968c9-112">ใน**นโยบายที่นำไปใช้กับส่วนทั้งหมดขององค์กร**ให้เลือกนโยบายแล้วคลิก**แก้ไข**</span><span class="sxs-lookup"><span data-stu-id="968c9-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="968c9-113">ภายใต้**การตั้งค่า**ให้เปิดใช้งาน**ลิงก์ที่ปลอดภัยไปยังข้อความที่ส่งภายในองค์กร**</span><span class="sxs-lookup"><span data-stu-id="968c9-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
