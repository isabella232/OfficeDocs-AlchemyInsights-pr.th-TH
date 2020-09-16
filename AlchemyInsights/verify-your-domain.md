---
title: ยืนยันโดเมนของคุณ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734325"
---
# <a name="verify-your-domain"></a><span data-ttu-id="d62e3-102">ยืนยันโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="d62e3-102">Verify your domain</span></span>

 <span data-ttu-id="d62e3-103">**ระเบียนอาจยังไม่ได้รับการอัปเดตระหว่างอินเทอร์เน็ต**</span><span class="sxs-lookup"><span data-stu-id="d62e3-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="d62e3-104">โดยทั่วไปแล้วจะใช้เวลาเพียงไม่กี่นาทีเพื่อให้เราสามารถเห็นระเบียนใหม่ได้แต่ในบางครั้งอาจใช้เวลานานถึงสองสามชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="d62e3-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="d62e3-105">ถ้าคุณรออยู่แล้วให้ตรวจสอบอีกครั้งว่าคุณได้คัดลอกและวางค่าที่แน่นอนลงในระเบียนการตรวจสอบ TXT ที่โฮสต์ DNS ของคุณ</span><span class="sxs-lookup"><span data-stu-id="d62e3-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="d62e3-106">ปัญหาทั่วไปหนึ่งไม่รวมถึงส่วน "MS =" ของระเบียน</span><span class="sxs-lookup"><span data-stu-id="d62e3-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="d62e3-107">เราจำเป็นต้องใช้!</span><span class="sxs-lookup"><span data-stu-id="d62e3-107">We need that too!</span></span>

- <span data-ttu-id="d62e3-108">ที่โฮสต์ DNS บางอย่างคุณจำเป็นต้องทำขั้นตอนเพิ่มเติมเพื่อบันทึกไฟล์โซน (ที่เก็บระเบียน DNS ไว้) เพื่อที่จะอัปเดตระหว่างอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="d62e3-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="d62e3-109">ตรวจสอบให้แน่ใจว่าคุณได้บันทึกการเปลี่ยนแปลงของคุณแล้วเพื่อให้ Microsoft สามารถดูและตรวจสอบระเบียนได้</span><span class="sxs-lookup"><span data-stu-id="d62e3-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
