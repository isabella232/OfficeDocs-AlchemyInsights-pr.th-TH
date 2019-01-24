---
title: การแก้ไขปัญหาข้อผิดพลาดในการรับรองความถูกต้องขั้นตอน
ms.author: kaarins
author: kaarins
ms.date: 6/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: fbb2ea4f0c6e582dae71371d958667162a138346
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/24/2019
ms.locfileid: "29493496"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="f464c-102">การแก้ไขปัญหาข้อผิดพลาดในการรับรองความถูกต้องขั้นตอน</span><span class="sxs-lookup"><span data-stu-id="f464c-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="f464c-p101">ในหลายกรณี ขั้นตอนการล้มเหลวเนื่องจากมีข้อผิดพลาดในการรับรองความถูกต้อง ถ้าคุณมีข้อผิดพลาดชนิดนี้ ประกอบด้วยข้อผิดพลาด "Unauthorized" หรือรหัสข้อผิดพลาด 401 หรือ 403 ปรากฏขึ้น โดยปกติแล้วคุณสามารถแก้ไขข้อผิดพลาดการรับรองความถูกต้อง ด้วยการปรับปรุงการเชื่อมต่อ:</span><span class="sxs-lookup"><span data-stu-id="f464c-p101">In many cases, flows fail because of an authentication error. If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears. You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="f464c-106">ที่ด้านบนสุดของ web portal คลิ กหรือเลือกเกียร์ไอคอนเพื่อเปิดเมนูการตั้งค่า แล้วคลิ กหรือแตะเพื่อ**เชื่อมต่อ**</span><span class="sxs-lookup"><span data-stu-id="f464c-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="f464c-107">เลื่อนไปที่การเชื่อมต่อที่คุณเห็นข้อความข้อผิดพลาดที่ไม่ได้รับอนุญาต</span><span class="sxs-lookup"><span data-stu-id="f464c-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="f464c-108">ถัดจากการเชื่อมต่อ คลิ กหรือแตะเพื่อ**ผ่านการตรวจสอบ**การเชื่อมโยงในข้อความเกี่ยวกับการเชื่อมต่อที่ไม่มีการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="f464c-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="f464c-109">ตรวจสอบข้อมูลประจำตัวของคุณ โดยทำตามคำแนะนำที่ปรากฏ กลับไปยังความล้มเหลวของคุณรันขั้นตอน และจากนั้นคลิ กหรือแตะเพื่อ**ส่งอีกครั้ง**หรือไม่</span><span class="sxs-lookup"><span data-stu-id="f464c-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="f464c-110">สำหรับวิธีใช้เพิ่มเติม ดู[ขั้นตอนการแก้ไขปัญหา](https://go.microsoft.com/fwlink/?linkid=872110)</span><span class="sxs-lookup"><span data-stu-id="f464c-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

