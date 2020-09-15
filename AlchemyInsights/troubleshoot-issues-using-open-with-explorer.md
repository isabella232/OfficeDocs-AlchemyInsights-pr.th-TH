---
title: แก้ไขปัญหาการใช้เปิดด้วย Explorer
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659077"
---
# <a name="fix-problems-with-open-with-explorer"></a>แก้ไขปัญหาเกี่ยวกับการเปิดด้วย Explorer

แก้ไขปัญหาทั่วไปเกี่ยวกับการเปิดไลบรารีเอกสารใน SharePoint หรือ OneDrive โดยใช้คำสั่ง **เปิดด้วย Explorer** : 
  
- ใช้ Internet Explorer 10 หรือ Internet Explorer 11 **เปิดด้วย Explorer** ไม่เข้ากันได้กับ Microsoft Edge, Google Chrome, Firefox และผู้อื่น **เปิดด้วย Explorer** ถูกปิดใช้งานในเบราว์เซอร์ทั้งหมดยกเว้น Internet Explorer 
    
- **เปิดด้วย Explorer** ไม่พร้อมใช้งานในประสบการณ์การใช้งานที่ทันสมัยสำหรับไลบรารี SharePoint ใช้ **มุมมองใน File Explorer** แทน เลือกมุมมอง**ตัวเลือกมุมมอง** \> **ใน File Explorer** ดูใน File Explorer ไม่เข้ากันกับ Microsoft Edge, Google Chrome, Firefox และผู้อื่น **ดูใน File explorer** ที่พร้อมใช้งานเฉพาะใน Internet Explorer 
    
- ตรวจสอบให้แน่ใจว่าบริการ WebClient กำลังทำงานอยู่ ในกล่องค้นหาของ Windows ให้พิมพ์เรียกใช้เลือกแอปเรียกใช้เดสก์ท็อปพิมพ์ services. msc แล้วกด Enter เลื่อนลงไปยังบริการ WebClient และตรวจสอบให้แน่ใจว่าคอลัมน์ **สถานะ** แสดง "กำลังทำงาน" ถ้าไม่ใช่ให้ดับเบิลคลิกที่บริการนั้นแล้วคลิก**เริ่ม**แล้วคลิก**ตกลง** (คุณอาจจำเป็นต้องเปิดใช้งานบริการก่อนด้วยการเลือก **ด้วยตนเอง** หรือ **โดยอัตโนมัติ** ในกล่อง **ชนิดการเริ่มต้น** ) 
    
> [!NOTE]
> การเปิดไลบรารีใน File Explorer มีประโยชน์ในกรณีที่คุณต้องการคัดลอกหรือย้ายไฟล์และโฟลเดอร์หลายๆไฟล์แต่ถ้าคุณต้องการทำงานในไลบรารีเป็นประจำเราขอแนะนำให้ซิงค์ เมื่อต้องการแก้ไขปัญหาการเปิดใน File Explorer ให้ดูที่[เปิดใน Explorer](https://go.microsoft.com/fwlink/?linkid=871665) สำหรับข้อมูลเกี่ยวกับการตั้งค่าการซิงค์ให้ดู[ที่ซิงค์ไฟล์ SharePoint ด้วยไคลเอ็นต์การซิงค์ OneDrive ใหม่](https://go.microsoft.com/fwlink/?linkid=871666)
  
โปรดดูบทความ [วิธีใช้คำสั่ง "เปิดด้วย Explorer" เพื่อแก้ไขปัญหาใน SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) สำหรับข้อมูลเพิ่มเติม 
  

