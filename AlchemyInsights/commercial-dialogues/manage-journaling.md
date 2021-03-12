---
title: จัดการบันทึกช่วยบันทึก
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748667"
---
# <a name="manage-journaling"></a><span data-ttu-id="33efb-102">จัดการบันทึกช่วยบันทึก</span><span class="sxs-lookup"><span data-stu-id="33efb-102">Manage journaling</span></span>

<span data-ttu-id="33efb-103">การบันทึกข้อมูลการสื่อสารสามารถช่วยให้องค์กรของคุณตอบสนองต่อข้อกฎหมาย ข้อบังคับ และการปฏิบัติตามข้อบังคับขององค์กรได้ โดยการบันทึกการสื่อสารอีเมลขาเข้าและขาออก</span><span class="sxs-lookup"><span data-stu-id="33efb-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="33efb-104">โปรดทราบว่า:</span><span class="sxs-lookup"><span data-stu-id="33efb-104">Keep in mind:</span></span>

* <span data-ttu-id="33efb-105">คุณต้องมีสิทธิ์[การจัดการองค์กร](https://go.microsoft.com/fwlink/?linkid=2115259)[และการจัดการระเบียน](https://go.microsoft.com/fwlink/?linkid=2115469)ก่อนที่คุณจะสามารถจัดการการบันทึกข้อมูลบันทึกได้</span><span class="sxs-lookup"><span data-stu-id="33efb-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="33efb-106">คุณต้องมีกล่องจดหมายบันทึกรายวันและ (หรือ) กล่องจดหมายบันทึกอื่นที่กําหนดค่าไว้</span><span class="sxs-lookup"><span data-stu-id="33efb-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="33efb-107">เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[กําหนดค่าบันทึกการประชุมใน Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260)</span><span class="sxs-lookup"><span data-stu-id="33efb-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="33efb-108">ใน Exchange Online มีการจํากัดจํานวนกฎบันทึกรายวันที่คุณสามารถสร้างได้</span><span class="sxs-lookup"><span data-stu-id="33efb-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="33efb-109">For details, see [journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span><span class="sxs-lookup"><span data-stu-id="33efb-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="33efb-110">Exchange Online ไม่สนับสนุนการส่งรายงานบันทึกการประชุมไปยังกล่องจดหมาย Exchange Online</span><span class="sxs-lookup"><span data-stu-id="33efb-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="33efb-111">คุณต้องระบุที่อยู่อีเมลของระบบเก็บถาวรภายในองค์กรหรือบริการการเก็บถาวรของบริษัทอื่นเป็นกล่องจดหมายบันทึกรายวัน</span><span class="sxs-lookup"><span data-stu-id="33efb-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>
