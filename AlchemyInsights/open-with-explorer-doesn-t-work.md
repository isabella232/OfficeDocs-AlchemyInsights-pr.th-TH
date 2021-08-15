---
title: เปิดด้วย Explorer ไม่ใช้งาน
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
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011355"
---
# <a name="open-with-explorer-isnt-working"></a>เปิดด้วย Explorer ไม่ใช้งาน

ถ้า **เปิดด้วย Explorer** **หรือ ดูใน File Explorer** ไม่ผล ให้ตรวจสอบให้แน่ใจว่าบริการ WebClient ถูกตั้งค่าเป็น **เรียกใช้** โดยปฏิบัติตามขั้นตอนด้านล่าง ตัวอย่างเช่น อาจใช้เวลานานในการเปิดไลบรารี SharePoint OneDriveไลบรารีเมื่อบริการไม่ได้เรียกใช้อยู่ 
  
1. ในกล่องWindowsการค้นหา ให้พิมพ์ เรียกใช้ เลือกเรียกใช้แอปบนเดสก์ท็อป พิมพ์ services.msc **แล้วเลือก** Enter
    
2. เลื่อนลงไปยังบริการ WebClient แล้วตรวจดู **คอลัมน์** สถานะ ถ้าสถานะบริการ WebClient **ไม่ได้เรียกใช้****ดับเบิลคลิกที่บริการ** คลิก เริ่ม **แล้วคลิก** ตกลง เปิดใช้งานบริการ ถ้าต้องการ โดยการเลือก **ด้วยตนเอง****หรือ** อัตโนมัติ ในกล่อง **ชนิด** การเริ่มต้น 
    
> [!NOTE]
> เมื่อต้องการแก้ไขปัญหาในการเปิดใน File Explorer [ให้ดู เปิดใน](https://go.microsoft.com/fwlink/?linkid=871665)Explorer สรารวตการซิงค์เป็นทางเลือก[ที่ดีกว่า: SharePointไฟล์ด้วยไคลเอ็นต์การซิงค์สําหรับ OneDriveใหม่](https://go.microsoft.com/fwlink/?linkid=871666) 
  

