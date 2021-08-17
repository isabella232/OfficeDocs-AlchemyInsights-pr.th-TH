---
title: แก้ไขปัญหาโดยใช้ เปิดด้วย Explorer
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
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048175"
---
# <a name="fix-problems-with-open-with-explorer"></a>แก้ไขปัญหาเกี่ยวกับ เปิดด้วย Explorer

แก้ไขปัญหาทั่วไปเกี่ยวกับการเปิดไลบรารีเอกสารในไลบรารีSharePointหรือOneDriveใช้ **สั่ง เปิดด้วย Explorer:** 
  
- ใช้ Internet Explorer 10 หรือ Internet Explorer 11 **เปิดด้วย Explorer** เข้ากันไม่ได้กับ Microsoft Edge, Google Chrome, Firefox และอื่นๆ **เปิดด้วย Explorer** ถูกปิดใช้งานในเบราว์เซอร์ทั้งหมดยกเว้น Internet Explorer 
    
- **เปิดด้วย Explorer** ไม่พร้อมใช้งานในประสบการณ์ที่ทันสมัยSharePointไลบรารีของคุณ ใช้ **มุมมอง ใน File Explorer** แทน เลือก **ตัวเลือก** \> **มุมมอง ดูใน File Explorer** ดูใน File Explorer เข้ากันไม่ได้กับMicrosoft Edge, Google Chrome, Firefox และอื่นๆ **ดูใน File Explorer** ใน พร้อมใช้งานเฉพาะใน Internet Explorer 
    
- ตรวจสอบให้แน่ใจว่าบริการ WebClient เรียกใช้อยู่ ในกล่องโต้ตอบWindows ให้พิมพ์ เรียกใช้ เลือกเรียกใช้แอปบนเดสก์ท็อป พิมพ์ services.msc แล้วกด Enter เลื่อนลงไปยังบริการ WebClient และตรวจสอบให้แน่ใจว่าคอลัมน์ **สถานะ** แสดง "เรียกใช้" ถ้าไม่ ให้ดับเบิลคลิกที่บริการ **คลิก** เริ่ม **แล้วคลิก** ตกลง (คุณอาจต้องเปิดใช้งานบริการก่อนโดยการเลือก **ด้วยตนเอง** หรือ **อัตโนมัติ** ในกล่อง **ชนิด** การเริ่มต้น) 
    
> [!NOTE]
> การเปิดไลบรารีใน File Explorer มีประโยชน์ถ้าคุณต้องคัดลอกหรือย้ายไฟล์และโฟลเดอร์หลายรายการเพียงครั้งเดียว แต่ถ้าคุณต้องการใช้งานไลบรารีเป็นปกติ เราขอแนะนนะให้ซิงค์ เมื่อต้องการแก้ไขปัญหาในการเปิดใน File Explorer [ให้ดู เปิดใน](https://go.microsoft.com/fwlink/?linkid=871665)Explorer For info about setting up sync, see [Sync SharePoint files with the new การซิงค์สําหรับ OneDrive client](https://go.microsoft.com/fwlink/?linkid=871666).
  
โปรดดูบทความ[วิธีใช้สั่ง "เปิดด้วย Explorer" เพื่อแก้ไขปัญหาSharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)ของคุณ เพื่อดูข้อมูลเพิ่มเติม 
  

