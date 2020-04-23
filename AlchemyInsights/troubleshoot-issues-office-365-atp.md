---
title: แก้ไขปัญหาเกี่ยวกับการป้องกันภัยคุกคามขั้นสูงของ Office 365 (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766764"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="c674e-102">แก้ไขปัญหาเกี่ยวกับ ATP 365 ของ Office</span><span class="sxs-lookup"><span data-stu-id="c674e-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="c674e-103">**แจ้งความล่าช้ากับการส่งข้อความอีเมล**?</span><span class="sxs-lookup"><span data-stu-id="c674e-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="c674e-104">ลองใช้ตัวเลือกการจัดส่งแบบไดนามิกสําหรับนโยบายสิ่งที่แนบที่ปลอดภัย ATP ของคุณ</span><span class="sxs-lookup"><span data-stu-id="c674e-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="c674e-105">วิธีนี้จะหลีกเลี่ยงความล่าช้าในการส่งข้อความอีเมลในขณะที่ปกป้องผู้รับจากไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="c674e-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="c674e-106">**คุณต้องการรายงานค่าบวกที่ผิดพลาดหรือค่าลบเท็จ**หรือไม่?</span><span class="sxs-lookup"><span data-stu-id="c674e-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="c674e-107">ใช้ลิงก์นี้เพื่อส่งไฟล์ของคุณสําหรับการวิเคราะห์:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="c674e-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="c674e-108">**คุณทราบหรือไม่ว่าคุณสามารถเปิดใช้งานการป้องกัน ATP Safe Links สําหรับอีเมลที่ส่งระหว่างบุคคลในองค์กรของคุณ**ได้</span><span class="sxs-lookup"><span data-stu-id="c674e-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="c674e-109">ทําตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="c674e-109">Follow these steps:</span></span>
    1. <span data-ttu-id="c674e-110">ไปที่https://protection.office.comแล้วลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="c674e-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="c674e-111">ไปที่**ลิงก์ที่ปลอดภัย\*\*\*\*ของนโยบาย** > **การจัดการภัยคุกคาม** > </span><span class="sxs-lookup"><span data-stu-id="c674e-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="c674e-112">ภายใต้**นโยบาย ที่ใช้กับผู้รับที่ระบุ**ให้แก้ไข (หรือเพิ่ม) นโยบาย</span><span class="sxs-lookup"><span data-stu-id="c674e-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="c674e-113">เลือก**ใช้ลิงก์ที่ปลอดภัยกับข้อความที่ส่งภายในองค์กร**</span><span class="sxs-lookup"><span data-stu-id="c674e-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="c674e-114">บันทึกนโยบายและอนุญาตให้การเปลี่ยนแปลงของคุณทํางานผ่านศูนย์ข้อมูลของคุณประมาณ 30 นาที</span><span class="sxs-lookup"><span data-stu-id="c674e-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="c674e-115">เมื่อต้องการรับความช่วยเหลือเพิ่มเติมเกี่ยวกับ ATP ให้ดูที่[การป้องกันภัยคุกคามขั้นสูงของ Office 365](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="c674e-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>