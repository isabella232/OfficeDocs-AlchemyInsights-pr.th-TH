---
title: แก้ไขปัญหาข้อผิดพลาดของการรับรองความถูกต้อง
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3c4ad806ed446803d8c1e0ba17b3a06d591985d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690586"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="b5423-102">แก้ไขปัญหาข้อผิดพลาดของการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="b5423-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="b5423-103">ในหลายกรณีการไหลล้มเหลวเนื่องจากมีข้อผิดพลาดในการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="b5423-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="b5423-104">ถ้าคุณมีข้อผิดพลาดชนิดนี้ข้อความแสดงข้อผิดพลาดประกอบด้วย "ไม่ได้รับอนุญาต" หรือรหัสข้อผิดพลาดของ๔๐๑หรือ๔๐๓ปรากฏขึ้น</span><span class="sxs-lookup"><span data-stu-id="b5423-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="b5423-105">โดยปกติแล้วคุณสามารถแก้ไขข้อผิดพลาดการตรวจสอบความถูกต้องได้โดยการอัปเดตการเชื่อมต่อดังนี้</span><span class="sxs-lookup"><span data-stu-id="b5423-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="b5423-106">ที่ด้านบนของเว็บพอร์ทัลให้คลิกหรือแตะไอคอนรูปเฟืองเพื่อเปิดเมนูการตั้งค่าแล้วคลิกหรือแตะการ**เชื่อมต่อ**</span><span class="sxs-lookup"><span data-stu-id="b5423-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="b5423-107">เลื่อนไปยังการเชื่อมต่อที่คุณเห็นข้อความแสดงข้อผิดพลาดที่ไม่ได้รับอนุญาต</span><span class="sxs-lookup"><span data-stu-id="b5423-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="b5423-108">ถัดจากการเชื่อมต่อให้คลิกหรือแตะที่ลิงก์ **ตรวจสอบรหัสผ่าน** ในข้อความเกี่ยวกับการเชื่อมต่อที่ไม่ได้รับการรับรองความถูกต้อง</span><span class="sxs-lookup"><span data-stu-id="b5423-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="b5423-109">การตรวจสอบข้อมูลประจำตัวของคุณโดยทำตามคำแนะนำที่ปรากฏขึ้นให้กลับไปยังความล้มเหลวในการทำงานของการทำงานของคุณแล้วคลิ**กหรือแตะส่ง**</span><span class="sxs-lookup"><span data-stu-id="b5423-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="b5423-110">สำหรับความช่วยเหลือเพิ่มเติมให้ดู[ที่การแก้ไขปัญหาการไหล](https://go.microsoft.com/fwlink/?linkid=872110)</span><span class="sxs-lookup"><span data-stu-id="b5423-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

