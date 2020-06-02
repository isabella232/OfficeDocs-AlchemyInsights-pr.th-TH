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
ms.openlocfilehash: f1dc675c8a8217ea2824ad46e029bfa303303e6a
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511131"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="8d048-102">แก้ไขปัญหาเกี่ยวกับ Atp ของ Office 365</span><span class="sxs-lookup"><span data-stu-id="8d048-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="8d048-103">**แจ้งความล่าช้ากับการส่งข้อความอีเมล์**?</span><span class="sxs-lookup"><span data-stu-id="8d048-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="8d048-104">ลองใช้ตัวเลือกการจัดส่งแบบไดนามิกสําหรับนโยบายสิ่งที่แนบมาที่ปลอดภัย ATP ของคุณ</span><span class="sxs-lookup"><span data-stu-id="8d048-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="8d048-105">การทําเช่นนี้จะหลีกเลี่ยงความล่าช้าในการจัดส่งข้อความอีเมลในขณะที่ปกป้องผู้รับจากแฟ้มที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="8d048-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="8d048-106">**คุณต้องการรายงานผลบวกเท็จหรือเชิงลบเท็จ**หรือไม่</span><span class="sxs-lookup"><span data-stu-id="8d048-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="8d048-107">ใช้ลิงก์นี้เพื่อส่งไฟล์ของคุณสําหรับการวิเคราะห์:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="8d048-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="8d048-108">**คุณทราบหรือไม่ว่าคุณสามารถเปิดใช้งานการป้องกันการเชื่อมโยงที่ปลอดภัยของ ATP สําหรับอีเมลที่ส่งระหว่างคนในองค์กรของคุณ**?</span><span class="sxs-lookup"><span data-stu-id="8d048-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="8d048-109">ทําตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="8d048-109">Follow these steps:</span></span>
    1. <span data-ttu-id="8d048-110">ไปที่ https://protection.office.com และลงชื่อเข้าใช้</span><span class="sxs-lookup"><span data-stu-id="8d048-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="8d048-111">ไปที่นโยบาย**การจัดการภัยคุกคาม**  >  **Policy**  >  **การเชื่อมโยงที่ปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="8d048-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="8d048-112">ภายใต้**นโยบายที่ใช้กับผู้รับที่ระบุ**ให้แก้ไข (หรือเพิ่ม) นโยบาย</span><span class="sxs-lookup"><span data-stu-id="8d048-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="8d048-113">เลือก**ใช้การเชื่อมโยงที่ปลอดภัยกับข้อความที่ส่งภายในองค์กร**</span><span class="sxs-lookup"><span data-stu-id="8d048-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="8d048-114">บันทึกนโยบายของคุณ และอนุญาตให้ประมาณ 30 นาทีเพื่อให้การเปลี่ยนแปลงของคุณทํางานผ่านศูนย์ข้อมูลของคุณ</span><span class="sxs-lookup"><span data-stu-id="8d048-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="8d048-115">เมื่อต้องการรับความช่วยเหลือเพิ่มเติมเกี่ยวกับ ATP ให้ดูที่[การป้องกันภัยคุกคามขั้นสูงของ Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="8d048-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/microsoft-365/security/office-365-security/office-365-atp).</span></span>