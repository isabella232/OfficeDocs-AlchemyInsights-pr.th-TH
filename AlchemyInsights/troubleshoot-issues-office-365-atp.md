---
title: แก้ไขปัญหากับ Office 365 ขั้นสูงคุกคามป้องกัน (ATP)
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dbdfe2ddcc4afd4477f66ffd060ddb7093af8fd6
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031120"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a><span data-ttu-id="1f671-102">แก้ไขปัญหาเกี่ยวกับ Office 365 ATP</span><span class="sxs-lookup"><span data-stu-id="1f671-102">Troubleshoot issues with Office 365 ATP</span></span>

- <span data-ttu-id="1f671-103">**ความล่าช้าในการแจ้งให้ทราบ ด้วยการส่งข้อความอีเมล**หรือไม่</span><span class="sxs-lookup"><span data-stu-id="1f671-103">**Notice delays with email message delivery**?</span></span> <span data-ttu-id="1f671-104">ลองใช้ตัวเลือกการจัดส่งแบบไดนามิกสำหรับนโยบาย ATP เซฟสิ่งที่แนบมาของคุณ</span><span class="sxs-lookup"><span data-stu-id="1f671-104">Try using the Dynamic Delivery option for your ATP Safe Attachments policies.</span></span> <span data-ttu-id="1f671-105">ซึ่งจะช่วยหลีกเลี่ยงความล่าช้าที่ส่งข้อความอีเมล โดยผู้รับจากแฟ้มที่เป็นอันตราย</span><span class="sxs-lookup"><span data-stu-id="1f671-105">This will avoid email message delivery delays while protecting recipients from malicious files.</span></span>
- <span data-ttu-id="1f671-106">**คุณต้องการทำงานผิดพลาด false รายงานหรือ false ค่าลบ**หรือไม่</span><span class="sxs-lookup"><span data-stu-id="1f671-106">**Do you want to report false positives or false negatives**?</span></span> <span data-ttu-id="1f671-107">ใช้การเชื่อมโยงนี้เพื่อส่งแฟ้มของคุณสำหรับการวิเคราะห์:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span><span class="sxs-lookup"><span data-stu-id="1f671-107">Use this link to submit your file for analysis: [https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)</span></span>
- <span data-ttu-id="1f671-108">**คุณทราบว่า คุณสามารถเปิดใช้งานการป้องกันเชื่อมโยงเซฟ ATP สำหรับอีเมลที่ส่งระหว่างผู้คนในองค์กรของคุณ**ได้อย่างไร</span><span class="sxs-lookup"><span data-stu-id="1f671-108">**Did you know that you can enable ATP Safe Links protection for email sent between people in your organization**?</span></span> <span data-ttu-id="1f671-109">ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="1f671-109">Follow these steps:</span></span>
    1. <span data-ttu-id="1f671-110">ไปที่https://protection.office.comและเข้าสู่ระบบ</span><span class="sxs-lookup"><span data-stu-id="1f671-110">Go to https://protection.office.com, and sign in.</span></span>
    2. <span data-ttu-id="1f671-111">**จัดการความเสี่ยง**ไป > **นโยบาย** > **การเชื่อมโยงที่ปลอดภัย**</span><span class="sxs-lookup"><span data-stu-id="1f671-111">Go to **Threat management** > **Policy** > **Safe Links**.</span></span>
    3. <span data-ttu-id="1f671-112">ภายใต้**นโยบายที่นำไปใช้กับผู้รับที่ระบุ**แก้ไข (หรือเพิ่ม) นโยบาย</span><span class="sxs-lookup"><span data-stu-id="1f671-112">Under **Policies that apply to specific recipients**, edit (or add) a policy.</span></span>
    4. <span data-ttu-id="1f671-113">เลือกการ**เชื่อมโยงเซฟนำไปใช้กับข้อความที่ส่งภายในองค์กร**</span><span class="sxs-lookup"><span data-stu-id="1f671-113">Select **Apply safe links to messages sent within the organization**.</span></span>
    5. <span data-ttu-id="1f671-114">บันทึกนโยบายของคุณ และอนุญาตให้ประมาณ 30 นาทีสำหรับการเปลี่ยนแปลงการทำงานของพวกเขารวด datacenter ของคุณ</span><span class="sxs-lookup"><span data-stu-id="1f671-114">Save your policy, and allow about 30 minutes for your changes to work their way through your datacenter.</span></span>
- <span data-ttu-id="1f671-115">เมื่อต้องการขอความช่วยเหลือเพิ่มเติมเกี่ยวกับ ATP ดู[การป้องกันภัยคุกคามขั้นสูงของ Office 365](https://docs.microsoft.com/office365/securitycompliance/office-365-atp)</span><span class="sxs-lookup"><span data-stu-id="1f671-115">To get more help with ATP, see [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).</span></span>