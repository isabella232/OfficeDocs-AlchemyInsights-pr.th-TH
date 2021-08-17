---
title: เหมือนกับชื่อไฟล์ที่ดีที่สุด
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312844"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"ต้องใช้งาน Alchemy Header H1, H2 ใช้งานไม่ได้"
หลักปฏิบัติที่ดีที่สุดและแนวทางของการเขียน Alchemy:

1. **อย่าซ้อน Alchemy Insightsอยู่ในโฟลเดอร์**- ตัวเลือกนี้จะตัดโครงสร้าง URL เราพยายามแก้ไขปัญหานี้
1. ไฟล์ในโฟลเดอร์ **AlchemyInsights** ควรมีชื่อไฟล์แบบพิมพ์เล็กที่มีเครื่องหมายยัติภังค์ในช่องว่าง เช่น **_how-to-enable-litigation-hold_**.
    1. รวม ID กฎหรือ ID กลุ่มจากพอร์ทัล [คู่ค้า Alchemy](https://alchemyportal.azurewebsites.net) ในเขตข้อมูล ms.custom เช่น ***ms.custom: 100021***
1. ใช้ Metadata ที่เหลือที่ด้านบนของไฟล์นี้เป็นเทมเพลตของคุณ
1. ใน [พอร์ทัลคู่ค้า Alchemy](https://alchemyportal.azurewebsites.net)ให้นําทางไปยังส่วน ชื่อข้อมูลเชิงลึกของลูกค้า **:** และใช้ชื่อนั้นเป็นจุดเริ่มต้นในชื่อ H1 ของคุณเพื่อให้เข้าใจข้อมูลเชิงลึก 

**หมายเหตุ**: Alchemy Insightsต้องมีเพียง H1 เดียวที่ด้านบนหรือจะหยุดการผลิต H2 ไม่แสดง ดังนั้น ให้ใช้ตัว **หนา** หรือรูปแบบอื่นๆ เพื่อแสดงส่วนที่แยกต่างหาก
1. ถัดไป ให้กรอกข้อความเนื้อหาโดยใช้เนื้อหาแบบร่างในส่วนCustomer Insightsของหน้ากฎ Alchemy
    1. รายการสัญลักษณ์แสดงหัวข้อย่อยนั้นใช้ได้ดี
    1. รายการล.ก. ด้วย
    1. **ตัว***หนาและตัว* เอียงก็ไม่เป็นไร
    1. ลิงก์ควรเป็น "ลิงก์ไปยัง **เว็บ"/ลิงก์ภายนอก** หรือ **ลิงก์ไปยังองค์ประกอบ UI** เสมอ ไม่ใช่ลิงก์ภายใน
    1. ขณะนี้ยังไม่รองรับรูปภาพอย่างเป็นทางการ แต่อยู่ในโรดแมป

และนี่เป็นเวลานานเกินไปจริงๆ แนวทางปฏิบัติที่ดีที่สุดคืออักขระประมาณ 400 ---------------------------------

เมื่อเนื้อหาของคุณพร้อมแล้ว ให้ดึงเนื้อหาไปยัง Live Branch จากนั้นไปที่พอร์ทัลคู่ค้า [Alchemy](https://alchemyportal.azurewebsites.net) และใส่ชื่อไฟล์ลงในเขตข้อมูล URL 