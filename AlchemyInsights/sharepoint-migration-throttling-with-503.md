---
title: การโยกย้าย SharePoint ที่มีข้อผิดพลาด๕๐๓
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: e46c39652db6a13a45d77d303102b4873e67a076
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720080"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>การโยกย้าย SharePoint ที่มีข้อผิดพลาด๕๐๓

**สำคัญ**: ในช่วงเวลาที่เป็นประวัติการณ์เหล่านี้เราจะดำเนินการตามขั้นตอนเพื่อให้แน่ใจว่าบริการ sharepoint Online และ OneDrive ยังคงพร้อมใช้งานอย่างมาก–โปรดไปที่การ [ปรับปรุงฟีเจอร์ชั่วคราวของ sharepoint Online](https://aka.ms/ODSPAdjustments) สำหรับข้อมูลเพิ่มเติม

**ข้อผิดพลาด๕๐๓เมื่อโยกย้ายไปยัง SharePoint Online**

แสดงว่าคุณกำลังโยกย้ายไปยัง SharePoint Online และได้รับข้อผิดพลาด๕๐๓ โปรดทำตามขั้นตอนด้านล่างเพื่อให้เราสามารถช่วยคุณได้โดยเร็วที่สุดเท่าที่จะเป็นไปได้ 

1. คลิก**ติดต่อฝ่ายสนับสนุน**แล้วคลิก**คำขอบริการใหม่**
2. สำหรับชื่อเรื่องและคำอธิบายให้พิมพ์การ**โยกย้าย SharePoint ที่ควบคุมปริมาณด้วย๕๐๓**
3. เมื่อมีการส่งตั๋วแล้วโปรดอัปเดตข้อมูลดังต่อไปนี้:
    - จำนวนครั้งที่เหลือของการโยกย้าย (ตัวอย่างเช่นกี่ช้อนโต๊ะ)
    - วันที่เริ่มต้นและวันที่สิ้นสุดการโยกย้าย
    - อธิบายว่าคุณกำลังโยกย้ายเนื้อหาของคุณจากที่ใดเช่น SharePoint Server กล่อง GDrive การแชร์ไฟล์และอื่นๆ
    - ประเมินจำนวนข้อผิดพลาดในการควบคุมปริมาณ (ตัวอย่างเช่น x throttle ต่อชั่วโมงหรือไม่) และเมื่อใดที่การควบคุมปริมาณเกิดขึ้น
    - เครื่องมือการโยกย้ายแบบใดที่คุณกำลังใช้ (ตัวอย่างเช่น SPMT หรือ ShareGate)


