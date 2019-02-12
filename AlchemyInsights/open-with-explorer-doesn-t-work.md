---
title: เปิด ด้วย Explorer ไม่ทำงาน
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906823"
---
# <a name="open-with-explorer-isnt-working"></a>เปิด ด้วย Explorer ไม่ได้ทำงาน

ถ้า**เปิด ด้วย Explorer**หรือ**มุมมองใน Explorer แฟ้ม**ทำงานไม่ ตรวจสอบว่า บริการ WebClient ถูกตั้งค่าให้**เรียกใช้**โดยทำตามขั้นตอนด้านล่างนี้ ตัวอย่างเช่น ดังกล่าวอาจใช้เวลานานเมื่อต้องการเปิดไลบรารี SharePoint หรือ OneDrive เมื่อไม่ได้ทำงานการบริการ 
  
1. ในกล่องค้นหาของ Windows ชนิดทำงาน เลือกเรียกใช้แอพลิเคชันเดสก์ท็อป ชนิด services.msc และจากนั้นเลือก**Enter**
    
2. เลื่อนลงไปยังบริการ WebClient และตรวจสอบคอลัมน์**สถานะ** ถ้าสถานะของบริการ WebClient ไม่**ทำงาน**คลิกสองครั้งที่บริการ คลิก**เริ่ม**และจากนั้น คลิก**ตกลง** เปิดใช้งานการบริการ ถ้าจำเป็น โดยเลือกอย่างใดอย่างหนึ่ง**ด้วยตนเอง**หรือ**โดยอัตโนมัติ**ในกล่อง**ชนิดการเริ่มต้น** 
    
> [!NOTE]
> เมื่อต้องการแก้ไขปัญหาที่เปิดในแฟ้ม Explorer ดู[เปิดใน Explorer](https://go.microsoft.com/fwlink/?linkid=871665) สำรวจข้อมูลให้ตรงกันเป็นทางเลือกดีกว่า: [SharePoint ซิงค์แฟ้มกับไคลเอนต์ซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666) 
  

