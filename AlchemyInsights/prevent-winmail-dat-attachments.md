---
title: ๒๕๘๙ช่วยป้องกันสิ่งที่แนบมาของ Winmail.dat ในข้อความอีเมลจากองค์กรของคุณ
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: f67c4146af419a590651c8e0673fd59fabd7eae7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47693754"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="ecd50-102">ช่วยป้องกันสิ่งที่แนบมาของ Winmail.dat ในข้อความอีเมลจากองค์กรของคุณ</span><span class="sxs-lookup"><span data-stu-id="ecd50-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="ecd50-103">ในฐานะผู้ดูแลระบบให้ลองทำตามขั้นตอนต่อไปนี้:</span><span class="sxs-lookup"><span data-stu-id="ecd50-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="ecd50-104">เปิด[ศูนย์การจัดการ Exchange](https://outlook.office365.com/ecp/)</span><span class="sxs-lookup"><span data-stu-id="ecd50-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="ecd50-105">ไปที่**Mail flow**  >  **โดเมนระยะไกล**ของจดหมายเวียน</span><span class="sxs-lookup"><span data-stu-id="ecd50-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="ecd50-106">เลือกโดเมนระยะไกลเริ่มต้นที่ชื่อ**ค่าเริ่ม**ต้นแล้วคลิก**แก้ไข**</span><span class="sxs-lookup"><span data-stu-id="ecd50-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="ecd50-107">ในส่วน **ใช้รูปแบบ Rich text** ให้เลือก **ไม่**มี</span><span class="sxs-lookup"><span data-stu-id="ecd50-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="ecd50-108">สำหรับข้อมูลเพิ่มเติมให้ดู[ที่ระบุรูปแบบข้อความสำหรับโดเมนระยะไกล](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format)</span><span class="sxs-lookup"><span data-stu-id="ecd50-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
