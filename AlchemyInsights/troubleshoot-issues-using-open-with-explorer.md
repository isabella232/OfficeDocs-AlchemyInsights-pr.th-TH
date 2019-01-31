---
title: แก้ปัญหาโดยใช้เปิด ด้วย Explorer
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: c95f07b9fb7251442577c014e4005dbe3f92ceb4
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661770"
---
# <a name="fix-problems-with-open-with-explorer"></a>แก้ปัญหาเกี่ยวกับการเปิดด้วย Explorer

แก้ไขปัญหาทั่วไปเกี่ยวกับการเปิดไลบรารีเอกสารใน SharePoint หรือ OneDrive โดยใช้คำสั่ง**เปิด ด้วย Explorer** : 
  
- ใช้ Internet Explorer 10 หรือ Internet Explorer 11 **เปิด ด้วย Explorer**ไม่เข้ากันกับ Microsoft ขอบ Google โครเมียม Firefox และผู้อื่น **เปิด ด้วย Explorer**ถูกปิดใช้งานในเบราว์เซอร์ทั้งหมดยกเว้น Internet Explorer 
    
- **เปิด ด้วย Explorer**จะไม่พร้อมใช้งานในประสบการณ์ใช้งานแบบสมัยใหม่สำหรับไลบรารี SharePoint ใช้**มุมมองใน Explorer แฟ้ม**แทน เลือก**ตัวเลือกมุมมอง** \> **มุมมอง Explorer แฟ้ม** มุมมองใน Explorer แฟ้มเข้ากันไม่ได้กับ ขอบของ Microsoft, Google โครเมียม Firefox และอื่น ๆ **มุมมองใน Explorer แฟ้ม**ในพร้อมใช้งานเฉพาะใน Internet Explorer 
    
- ตรวจสอบให้แน่ใจว่า กำลังเรียกใช้บริการ WebClient ใน Windows กล่องค้นหา ชนิดทำงาน เลือกเรียกใช้เดสก์ท็อปแอพลิเคชัน พิมพ์ services.msc และจากนั้น กด Enter เลื่อนลงไปยังบริการ WebClient และต้องแน่ใจว่า คอลัมน์**สถานะ**แสดง "รัน" หากโปรแกรมไม่ คลิกสองครั้งที่บริการ คลิก**เริ่ม**และจากนั้น คลิก**ตกลง** (คุณอาจจำเป็นต้องเปิดใช้งานการบริการก่อน โดยเลือกอย่างใดอย่างหนึ่ง**ด้วยตนเอง**หรือ**โดยอัตโนมัติ**ในกล่อง**ชนิดการเริ่มต้นระบบ**) 
    
> [!NOTE]
> เปิดไลบรารีในแฟ้ม Explorer จะสะดวกถ้าคุณต้องการคัดลอก หรือย้ายแฟ้มและโฟลเดอร์หลายทันที แต่ ถ้าคุณต้องการทำงานเป็นประจำในไลบรารี เราขอแนะนำให้ตรงกัน เมื่อต้องการแก้ไขปัญหาที่เปิดในแฟ้ม Explorer ดู[เปิดใน Explorer](https://go.microsoft.com/fwlink/?linkid=871665) สำหรับข้อมูลเกี่ยวกับการตั้งค่าการซิงค์ ดู[SharePoint ซิงค์แฟ้มกับไคลเอนต์ซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666)
  
โปรดดูบทความ[วิธีใช้คำสั่ง "เปิดด้วย Explorer " การแก้ไขปัญหาใน SharePoint แบบออนไลน์](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)สำหรับข้อมูลเพิ่มเติม 
  

