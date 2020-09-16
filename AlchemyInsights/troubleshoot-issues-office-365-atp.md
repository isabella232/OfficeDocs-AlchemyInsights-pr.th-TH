---
title: การแก้ไขปัญหาเกี่ยวกับ Office ๓๖๕การป้องกันการคุกคามขั้นสูง (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 4164781a331ec919811332e94636449e9d88430d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758084"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="3fcf8-102">การแก้ไขปัญหาเกี่ยวกับ Office ๓๖๕ ATP</span><span class="sxs-lookup"><span data-stu-id="3fcf8-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="3fcf8-103">การ**แจ้งเตือนล่าช้าด้วยการส่งข้อความอีเมล**</span><span class="sxs-lookup"><span data-stu-id="3fcf8-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="3fcf8-104">ลองใช้ตัวเลือกการนำส่งแบบไดนามิกสำหรับนโยบายสิ่งที่แนบมาของ ATP Safe ของคุณ</span><span class="sxs-lookup"><span data-stu-id="3fcf8-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="3fcf8-105">วิธีนี้จะหลีกเลี่ยงความล่าช้าในการนำส่งข้อความอีเมลในขณะที่ปกป้องผู้รับจากไฟล์ที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="3fcf8-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="3fcf8-106">**คุณต้องการรายงาน false บวกหรือ**ค่าลบ false หรือไม่</span><span class="sxs-lookup"><span data-stu-id="3fcf8-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="3fcf8-107">ใช้ลิงก์นี้เพื่อส่งไฟล์ของคุณสำหรับการวิเคราะห์: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="3fcf8-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="3fcf8-108">**คุณทราบหรือไม่ว่าคุณสามารถเปิดใช้งานการป้องกันการเชื่อมโยงที่ปลอดภัยของ ATP สำหรับอีเมลที่ส่งระหว่างบุคคลในองค์กรของคุณ**</span><span class="sxs-lookup"><span data-stu-id="3fcf8-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="3fcf8-109">ให้ทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="3fcf8-109">Follow these steps:</span></span>
    1. <span data-ttu-id="3fcf8-110">ไปที่ https://protection.office.com แล้วลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="3fcf8-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="3fcf8-111">ไปที่**Threat management**  >  **Policy**  >  **ลิงก์ความปลอดภัย**ของนโยบายการจัดการภัยคุกคาม</span><span class="sxs-lookup"><span data-stu-id="3fcf8-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="3fcf8-112">ภายใต้ **นโยบายที่นำไปใช้กับผู้รับที่ระบุ**แก้ไข (หรือเพิ่ม) นโยบาย</span><span class="sxs-lookup"><span data-stu-id="3fcf8-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="3fcf8-113">เลือก**นำลิงก์ที่ปลอดภัยไปใช้กับข้อความที่ส่งภายในองค์กร**</span><span class="sxs-lookup"><span data-stu-id="3fcf8-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="3fcf8-114">บันทึกนโยบายของคุณและอนุญาตให้ใช้เวลาประมาณ30นาทีเพื่อให้การเปลี่ยนแปลงของคุณทำงานผ่านทางศูนย์ข้อมูลของคุณ</span><span class="sxs-lookup"><span data-stu-id="3fcf8-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="3fcf8-115">เมื่อต้องการรับความช่วยเหลือเพิ่มเติมเกี่ยวกับ ATP ให้ดูที่[การป้องกันการคุกคามขั้นสูงของ Office ๓๖๕](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="3fcf8-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>