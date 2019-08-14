---
title: 2589 ป้องกันสิ่งที่แนบ Winmail.dat ในข้อความอีเมลจากองค์กรของคุณ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: 41ab3f22499994cda5883834ff54e5767c69265b
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391579"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="207ff-102">ช่วยป้องกันสิ่งที่แนบ Winmail.dat ในข้อความอีเมลจากองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="207ff-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="207ff-103">เป็นการดูแล ทำตามขั้นตอนเหล่านี้:</span><span class="sxs-lookup"><span data-stu-id="207ff-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="207ff-104">เปิด[ศูนย์ดูแลอัตราแลกเปลี่ยน](https://outlook.office365.com/ecp/)</span><span class="sxs-lookup"><span data-stu-id="207ff-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="207ff-105">**การรับส่งจดหมาย**ไป > **โดเมนระยะไกล**</span><span class="sxs-lookup"><span data-stu-id="207ff-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="207ff-106">เลือกโดเมนระยะไกลเริ่มต้นชื่อ**เริ่มต้น**และจากนั้น คลิก**แก้ไข**</span><span class="sxs-lookup"><span data-stu-id="207ff-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="207ff-107">ในส่วนของการ**จัดรูปแบบข้อความ rich Text ใช้**เลือก**ไม่**</span><span class="sxs-lookup"><span data-stu-id="207ff-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="207ff-108">สำหรับข้อมูลเพิ่มเติม ให้ดู[ระบุรูปแบบข้อความสำหรับโดเมนระยะไกล](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format)</span><span class="sxs-lookup"><span data-stu-id="207ff-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
