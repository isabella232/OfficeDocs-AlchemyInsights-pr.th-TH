---
title: เปิดด้วย Explorer ไม่ทำงาน
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694475"
---
# <a name="open-with-explorer-isnt-working"></a>เปิดด้วย Explorer ไม่ทำงาน

ถ้า **เปิดด้วย Explorer** หรือ **มุมมองใน File Explorer** ไม่ทำงานให้ตรวจสอบให้แน่ใจว่าบริการ WebClient ถูกตั้งค่าให้ **ทำงานโดยทำ** ตามขั้นตอนด้านล่างนี้ ตัวอย่างเช่นอาจใช้เวลานานในการเปิดไลบรารี SharePoint หรือ OneDrive เมื่อบริการไม่ได้ทำงานอยู่ 
  
1. ในกล่องค้นหาของ Windows ให้พิมพ์เรียกใช้เลือกแอปเรียกใช้เดสก์ท็อปพิมพ์ services. msc แล้วเลือก**Enter**
    
2. เลื่อนลงไปยังบริการ WebClient แล้วตรวจสอบคอลัมน์**สถานะ** ถ้าสถานะบริการ WebClient ไม่ได้**ทำงาน**อยู่ให้ดับเบิลคลิกที่บริการดังกล่าวแล้วคลิก**เริ่ม**แล้วคลิก**ตกลง** เปิดใช้งานบริการถ้าจำเป็นโดยเลือก**ด้วยตนเอง**หรือ**โดยอัตโนมัติ**ในกล่อง**ชนิดการเริ่มต้น** 
    
> [!NOTE]
> เมื่อต้องการแก้ไขปัญหาการเปิดใน File Explorer ให้ดูที่[เปิดใน Explorer](https://go.microsoft.com/fwlink/?linkid=871665) สำรวจการซิงค์เป็นทางเลือกที่ดียิ่งขึ้น:[ซิงค์ไฟล์ SharePoint กับไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666) 
  

