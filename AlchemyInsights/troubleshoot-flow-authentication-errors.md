---
title: การแก้ไขปัญหาข้อผิดพลาดของการตรวจสอบสิทธิ์โฟลว์
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 70451f074a65a4454faeadd188a31783be8e6c7e
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759747"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="83bf8-102">การแก้ไขปัญหาข้อผิดพลาดของการตรวจสอบสิทธิ์โฟลว์</span><span class="sxs-lookup"><span data-stu-id="83bf8-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="83bf8-103">ในหลายกรณี โฟลว์ล้มเหลวเนื่องจากมีข้อผิดพลาดการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="83bf8-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="83bf8-104">ข้อความแสดงข้อผิดพลาดประกอบด้วย "ไม่ได้รับอนุญาต" หรือรหัสข้อผิดพลาดของ 401 หรือ 403 ปรากฏขึ้น</span><span class="sxs-lookup"><span data-stu-id="83bf8-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="83bf8-105">โดยปกติแล้วคุณสามารถแก้ไขข้อผิดพลาดการรับรองความถูกต้องโดยการปรับปรุงการเชื่อมต่อ:</span><span class="sxs-lookup"><span data-stu-id="83bf8-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="83bf8-106">ที่ด้านบนของเว็บพอร์ทัล ให้คลิกหรือแตะไอคอนรูปเฟืองเพื่อเปิดเมนู การตั้งค่า แล้วคลิกหรือแตะ**การเชื่อมต่อ**</span><span class="sxs-lookup"><span data-stu-id="83bf8-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="83bf8-107">เลื่อนไปยังการเชื่อมต่อที่คุณเห็นข้อความแสดงข้อผิดพลาดที่ไม่ได้รับอนุญาต</span><span class="sxs-lookup"><span data-stu-id="83bf8-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="83bf8-108">ถัดจากการเชื่อมต่อ ให้คลิกหรือแตะลิงก์**ยืนยันรหัสผ่าน**ในข้อความเกี่ยวกับการเชื่อมต่อที่ไม่ถูกรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="83bf8-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="83bf8-109">ตรวจสอบข้อมูลประจําตัวของคุณโดยทําตามคําแนะนําที่ปรากฏ**Resubmit**</span><span class="sxs-lookup"><span data-stu-id="83bf8-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="83bf8-110">สําหรับวิธีใช้เพิ่มเติม ให้ดูที่[การแก้ไขปัญหาขั้นตอน](https://go.microsoft.com/fwlink/?linkid=872110)</span><span class="sxs-lookup"><span data-stu-id="83bf8-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

