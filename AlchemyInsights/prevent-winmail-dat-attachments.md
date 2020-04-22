---
title: 2589 ช่วยป้องกันสิ่งที่แนบมา Winmail.dat ในข้อความอีเมลจากองค์กรของคุณ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: 5336d4087e0a7579b68d6d97073726d020c89b47
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43666760"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="7a685-102">ช่วยป้องกันสิ่งที่แนบมาของ Winmail.dat ในข้อความอีเมลจากองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="7a685-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="7a685-103">ในฐานะผู้ดูแลระบบ ให้ลองทําตามขั้นตอนต่อไปนี้</span><span class="sxs-lookup"><span data-stu-id="7a685-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="7a685-104">เปิด[ศูนย์การจัดการ Exchange](https://outlook.office365.com/ecp/)</span><span class="sxs-lookup"><span data-stu-id="7a685-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="7a685-105">ไปที่**โดเมนระยะไกลของโฟล** > **ว์**จดหมาย</span><span class="sxs-lookup"><span data-stu-id="7a685-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="7a685-106">เลือกโดเมนเริ่มต้นระยะไกลที่ชื่อ**ค่าเริ่มต้น**แล้วคลิก**แก้ไข**</span><span class="sxs-lookup"><span data-stu-id="7a685-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="7a685-107">ในส่วน**ใช้รูปแบบ Rich-Text**ให้เลือก**ไม่**</span><span class="sxs-lookup"><span data-stu-id="7a685-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="7a685-108">สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การระบุรูปแบบข้อความสําหรับโดเมนระยะไกล](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format)</span><span class="sxs-lookup"><span data-stu-id="7a685-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
