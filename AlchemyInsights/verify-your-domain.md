---
title: ตรวจสอบว่า โดเมนของคุณ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d37cdae616fabd2813dc7c8074e94b05f0391d20
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2019
ms.locfileid: "28315952"
---
# <a name="verify-your-domain"></a><span data-ttu-id="a3b08-102">ตรวจสอบว่า โดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="a3b08-102">Verify your domain</span></span>

 <span data-ttu-id="a3b08-103">**เรกคอร์ดที่อาจจะยังไม่มีการปรับปรุงผ่านอินเทอร์เน็ต**</span><span class="sxs-lookup"><span data-stu-id="a3b08-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="a3b08-104">โดยทั่วไปเพียงใช้สักครู่เพื่อให้สามารถดูเรกคอร์ดใหม่ให้เรา แต่ในบางครั้งซึ่งอาจใช้เวลานานถึงสองสามชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="a3b08-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="a3b08-p101">ถ้าคุณเคยรอที่นานแล้ว ตรวจสอบว่า คุณได้คัดลอก และวางค่าที่แน่นอนในการตรวจสอบระเบียน TXT ที่โฮสต์ DNS ของคุณอีกครั้ง ปัญหาหนึ่งที่พบไม่ได้รวมถึงการ " MS =" เป็นส่วนหนึ่งของเรกคอร์ด เราต้องการที่มากเกินไป</span><span class="sxs-lookup"><span data-stu-id="a3b08-p101">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host. One common issue is not including the "MS=" part of the record. We need that too!</span></span>
    
- <span data-ttu-id="a3b08-p102">ในบางโฮสต์ DNS คุณจำเป็นต้องใช้มีขั้นตอนเพิ่มเติมเพื่อบันทึกแฟ้มโซน (ระเบียน DNS เก็บ) เพื่อที่จะปรับปรุงผ่านอินเทอร์เน็ต ตรวจสอบให้แน่ใจว่า คุณได้บันทึกการเปลี่ยนแปลงของคุณเพื่อให้ Office 365 สามารถมองเห็น และตรวจสอบเรกคอร์ด</span><span class="sxs-lookup"><span data-stu-id="a3b08-p102">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet. Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
    

