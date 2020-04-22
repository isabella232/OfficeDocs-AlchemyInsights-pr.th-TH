---
title: ยืนยันโดเมนของคุณ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710462"
---
# <a name="verify-your-domain"></a><span data-ttu-id="4ee1b-102">ยืนยันโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="4ee1b-102">Verify your domain</span></span>

 <span data-ttu-id="4ee1b-103">**เรกคอร์ดอาจยังไม่ได้ปรับปรุงทั่วทั้งอินเทอร์เน็ต**</span><span class="sxs-lookup"><span data-stu-id="4ee1b-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="4ee1b-104">โดยทั่วไปแล้วจะใช้เวลาเพียงไม่กี่นาทีเท่านั้นที่เราสามารถเห็นบันทึกใหม่ ได้ แต่บางครั้งอาจใช้เวลานานถึงสองสามชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="4ee1b-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="4ee1b-105">หากคุณรอนานแล้ว ให้ตรวจสอบอีกครั้งว่าได้คัดลอกและวางค่าที่แน่นอนลงในระเบียนการยืนยัน TXT ที่โฮสต์ DNS ของคุณ</span><span class="sxs-lookup"><span data-stu-id="4ee1b-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="4ee1b-106">ปัญหาทั่วไปหนึ่งไม่ได้รวมส่วน "MS=" ของเรกคอร์ด</span><span class="sxs-lookup"><span data-stu-id="4ee1b-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="4ee1b-107">เราต้องการมันด้วย!</span><span class="sxs-lookup"><span data-stu-id="4ee1b-107">We need that too!</span></span>

- <span data-ttu-id="4ee1b-108">ที่โฮสต์ DNS บางโฮสต์ คุณต้องทําตามขั้นตอนพิเศษเพื่อบันทึกไฟล์โซน (ที่บันทึก DNS ถูกเก็บไว้) เพื่อให้มีการปรับปรุงผ่านทางอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="4ee1b-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="4ee1b-109">ตรวจสอบให้แน่ใจว่าคุณได้บันทึกการเปลี่ยนแปลงของคุณไว้เพื่อให้ Microsoft สามารถดูและตรวจสอบระเบียนได้</span><span class="sxs-lookup"><span data-stu-id="4ee1b-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
