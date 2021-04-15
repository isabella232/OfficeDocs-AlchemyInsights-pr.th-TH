---
title: ยืนยันโดเมนของคุณ
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771010"
---
# <a name="verify-your-domain"></a><span data-ttu-id="f0678-102">ยืนยันโดเมนของคุณ</span><span class="sxs-lookup"><span data-stu-id="f0678-102">Verify your domain</span></span>

 <span data-ttu-id="f0678-103">**ระเบียนอาจไม่ได้อัปเดตทั่วทั้งอินเทอร์เน็ต**</span><span class="sxs-lookup"><span data-stu-id="f0678-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="f0678-104">โดยทั่วไปแล้วเราจะสามารถดูระเบียนใหม่ได้ภายในไม่กี่นาที แต่บางครั้งอาจใช้เวลานานถึงสองสามชั่วโมง</span><span class="sxs-lookup"><span data-stu-id="f0678-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="f0678-105">ถ้าคุณรอนานแล้ว ให้ตรวจสอบอีกครั้งว่าคุณได้คัดลอกและวางค่าที่ถูกต้องลงในระเบียนการตรวจสอบ TXT ที่โฮสต์ DNS ของคุณแล้ว</span><span class="sxs-lookup"><span data-stu-id="f0678-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="f0678-106">ปัญหาทั่วไปหนึ่งคือการไม่รวมส่วน "MS=" ของระเบียน</span><span class="sxs-lookup"><span data-stu-id="f0678-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="f0678-107">เราต้องการเช่นกัน!</span><span class="sxs-lookup"><span data-stu-id="f0678-107">We need that too!</span></span>

- <span data-ttu-id="f0678-108">ที่โฮสต์ DNS บางรายการ คุณจะต้องเพิ่มขั้นตอนในการบันทึกไฟล์โซน (ที่จัดเก็บระเบียน DNS ไว้) เพื่ออัปเดตทั่วทั้งอินเทอร์เน็ต</span><span class="sxs-lookup"><span data-stu-id="f0678-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="f0678-109">ตรวจสอบให้แน่ใจว่าคุณได้บันทึกการเปลี่ยนแปลงของคุณแล้ว เพื่อให้ Microsoft สามารถดูและตรวจสอบระเบียนได้</span><span class="sxs-lookup"><span data-stu-id="f0678-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
