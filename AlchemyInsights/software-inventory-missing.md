---
title: คลังซอฟต์แวร์หายไปหรือไม่ความไม่ถูกต้อง
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: f26fab92d0159c06eb600cf9ec4161892561a719e8d113d15bfbac133301e793
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897615"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>คลังซอฟต์แวร์หายไปหรือไม่ความไม่ถูกต้อง

คลังซอฟต์แวร์ใน การจัดการภัยคุกคามและช่องโหว่ (TVM) คือรายการซอฟต์แวร์ที่รู้จักในองค์กรของคุณที่มีการแจงนับแพลตฟอร์มทั่วไป (CPE) อย่างเป็นทางการ

ผลิตภัณฑ์ซอฟต์แวร์ที่ไม่มี CPE อย่างเป็นทางการไม่มีช่องโหว่ที่เผยแพร่ สินค้าคงคลังยังมีรายละเอียด เช่น ชื่อของผู้ขาย จํานวนของผู้โฆษณา ภัยคุกคาม และจํานวนอุปกรณ์ที่ถูกแสดง

การเปลี่ยนแปลงซอฟต์แวร์บนอุปกรณ์มักจะแสดงในพอร์ทัลความปลอดภัยภายในสองชั่วโมง อย่างไรก็ตาม บางครั้งอาจใช้เวลานานกว่านั้น ขณะนี้ยังไม่มีวิธีบังคับซิงค์ นี่คือแบบประเมินอย่างต่อเนื่อง

ถ้าคุณเปลี่ยนแปลงซอฟต์แวร์ และการเปลี่ยนแปลงใน TVM ไม่ถูกต้องหลังจากผ่านไป 5 ชั่วโมง ให้ปฏิบัติตามขั้นตอนเหล่านี้:

1. ตรวจสอบส่วนหลักฐานของซอฟต์แวร์เพื่อเข้าใจว่าซอฟต์แวร์ถูกตรวจพบอย่างไร
1. ตรวจสอบให้แน่ใจว่าซอฟต์แวร์ได้รับการสนับสนุน ซอฟต์แวร์อาจมองเห็นได้ในระดับอุปกรณ์เท่านั้น แม้ว่าซอฟต์แวร์ดังกล่าวไม่ได้รับการสนับสนุนในขณะนี้การจัดการภัยคุกคามและช่องโหว่อยู่ อย่างไรก็ตาม มีเฉพาะข้อมูลที่จํากัดเท่านั้น
1. For steps to report the inaccuracy from the portal, see [Report inaccuracy](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).
   
    **หมายเหตุ**: การรายงานความแม่นยําจากพอร์ทัล MDE คือช่องทางแบบทางเดียวสู่ทางวิศวกรรม หากปัญหาเร่งด่วน ให้เปิดตั๋วการสนับสนุน

For more information, see [Software inventory - การจัดการภัยคุกคามและช่องโหว่](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-software-inventory).