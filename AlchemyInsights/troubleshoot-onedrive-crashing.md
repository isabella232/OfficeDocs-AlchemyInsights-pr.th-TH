---
title: แก้ไขปัญหา OneDrive หยุดทำงาน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665017"
---
# <a name="troubleshoot-onedrive-crashes"></a>แก้ไขปัญหา OneDrive หยุดทำงาน

ถ้า OneDrive หยุดทำงานซ้ำๆให้ลองใช้ขั้นตอนการแก้ไขปัญหาต่อไปนี้:

**ตรวจสอบให้แน่ใจว่าไม่ได้ตั้งค่าคีย์รีจิสทรี:**

1. การใช้ Registry Editor ให้นำทางไปยัง HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. ถ้า DisableFileSyncNGSC มีอยู่และตั้งค่าเป็น1ให้เปิดคีย์และเปลี่ยนค่าเป็น0
3. เปิดใช้ OneDrive ด้วยตนเองโดยการไปที่เริ่ม ![กดแป้น Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)พิมพ์ OneDrive ในกล่องค้นหาจากนั้นคลิกที่แอป OneDrive บนเดสก์ท็อป

**ตั้งค่า OneDrive ใหม่:**

บันทึกย่อ

- การรีเซ็ต OneDrive จะยกเลิกการเชื่อมต่อการซิงค์ที่มีอยู่ทั้งหมด (รวมถึง OneDrive ส่วนบุคคลของคุณถ้าตั้งค่า)
- คุณจะไม่สูญเสียไฟล์หรือข้อมูลโดยการรีเซ็ต OneDrive บนคอมพิวเตอร์ของคุณ

**เมื่อต้องการตั้งค่า OneDrive ใหม่:**

1. เปิดกล่องโต้ตอบเรียกใช้โดยการกดแป้น Windows และ R
2. พิมพ์% localappdata% \Microsoft\OneDrive\onedrive.exe/reset แล้วกดตกลง หน้าต่างคำสั่งอาจปรากฏขึ้นสั้นๆ
3. เปิดใช้ OneDrive ด้วยตนเองโดยการไปที่เริ่ม ![กดแป้น Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)พิมพ์ OneDrive ในกล่องค้นหาจากนั้นคลิกที่แอป OneDrive บนเดสก์ท็อป

บันทึกย่อ

- ถ้าคุณเลือกที่จะซิงค์เฉพาะบางโฟลเดอร์ก่อนที่จะตั้งค่าใหม่คุณจะต้องดำเนินการดังกล่าวอีกครั้งเมื่อซิงค์เสร็จสมบูรณ์ อ่าน [เลือกโฟลเดอร์ OneDrive ที่จะซิงค์กับคอมพิวเตอร์ของคุณ](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   สำหรับข้อมูลเพิ่มเติม
- คุณจะต้องดำเนินการนี้ให้เสร็จสมบูรณ์สำหรับ OneDrive ส่วนบุคคลของคุณและ OneDrive for Business