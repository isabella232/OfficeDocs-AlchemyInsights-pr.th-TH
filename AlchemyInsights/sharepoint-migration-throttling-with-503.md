---
title: การควบคุมปริมาณการย้ายข้อมูลของ SharePoint ที่มีข้อผิดพลาด๕๐๓
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: d9d45b31afcc5ef68f5969117d08f0c8dcfe8850
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054072"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a>การควบคุมปริมาณการย้ายข้อมูลของ SharePoint ที่มีข้อผิดพลาด๕๐๓

ปรากฏขึ้นคุณกำลังโยกย้ายไปยัง SharePoint แบบออนไลน์และได้รับข้อผิดพลาด๕๐๓ โปรดทำตามขั้นตอนด้านล่างเพื่อให้เราสามารถช่วยเหลือคุณได้โดยเร็วที่สุด 

1. คลิกการ**สนับสนุนติดต่อ**และจากนั้นการ**ร้องขอการบริการใหม่**
2. สำหรับชื่อเรื่องและคำอธิบายให้พิมพ์**SharePoint การควบคุมปริมาณการโยกย้ายด้วย๕๐๓**
3. เมื่อส่งตั๋วแล้วโปรดอัปเดตข้อมูลดังต่อไปนี้:
    - จำนวนการย้ายข้อมูลที่เหลือ (ตัวอย่างเช่นจำนวน TBs เท่านั้น)
    - วันที่เริ่มต้นและสิ้นสุดการย้ายข้อมูล
    - อธิบายว่าคุณกำลังโยกย้ายเนื้อหาของคุณจากที่ใดเช่น SharePoint Server กล่อง GDrive, การแชร์ไฟล์ฯลฯ
    - ประมาณจำนวนข้อผิดพลาดในการควบคุมปริมาณ (ตัวอย่างเช่น x เค้นต่อชั่วโมง) และเมื่อใดที่การควบคุมปริมาณเกิดขึ้น
    - เครื่องมือการย้ายข้อมูลที่คุณใช้อยู่ (เช่น SPMT หรือ ShareGate)


