---
title: แก้ไขปัญหาข้อผิดพลาดในการรับรองความถูกต้อง
ms.author: pebaum
author: pebaum
ms.date: 6/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3d49d15d243dd98afc6f78b9e75f0cfa74c2cd7c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050652"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="df5a9-102">แก้ไขปัญหาข้อผิดพลาดในการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="df5a9-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="df5a9-103">ในหลายๆกรณีโฟลว์ล้มเหลวเนื่องจากมีข้อผิดพลาดในการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="df5a9-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="df5a9-104">หากคุณมีข้อผิดพลาดชนิดนี้แสดงว่าข้อผิดพลาดประกอบด้วย "ไม่ได้รับอนุญาต" หรือรหัสข้อผิดพลาดของ๔๐๑หรือ๔๐๓ปรากฏขึ้น</span><span class="sxs-lookup"><span data-stu-id="df5a9-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="df5a9-105">โดยปกติคุณสามารถแก้ไขข้อผิดพลาดการรับรองความถูกต้องโดยการปรับปรุงการเชื่อมต่อ:</span><span class="sxs-lookup"><span data-stu-id="df5a9-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="df5a9-106">ที่ด้านบนของเว็บพอร์ทัลให้คลิกหรือแตะไอคอนรูปเฟืองเพื่อเปิดเมนูการตั้งค่าแล้วคลิกหรือแตะการ**เชื่อมต่อ**</span><span class="sxs-lookup"><span data-stu-id="df5a9-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="df5a9-107">เลื่อนไปยังการเชื่อมต่อที่คุณเห็นข้อความข้อผิดพลาดที่ไม่ได้รับอนุญาต</span><span class="sxs-lookup"><span data-stu-id="df5a9-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="df5a9-108">ถัดจากการเชื่อมต่อให้คลิกหรือแตะลิงก์**ยืนยันรหัสผ่าน**ในข้อความเกี่ยวกับการเชื่อมต่อที่ไม่ได้รับการพิสูจน์ตัวตน</span><span class="sxs-lookup"><span data-stu-id="df5a9-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="df5a9-109">ตรวจสอบข้อมูลประจำตัวของคุณโดยทำตามคำแนะนำที่ปรากฏขึ้นให้กลับไปที่ความล้มเหลวในการไหลของคุณและจากนั้นคลิ**กหรือแตะส่งอีกครั้ง**</span><span class="sxs-lookup"><span data-stu-id="df5a9-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="df5a9-110">สำหรับความช่วยเหลือเพิ่มเติมโปรดดูที่[การแก้ไขปัญหาโฟลว์](https://go.microsoft.com/fwlink/?linkid=872110)</span><span class="sxs-lookup"><span data-stu-id="df5a9-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

