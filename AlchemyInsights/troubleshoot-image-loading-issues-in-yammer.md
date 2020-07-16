---
title: แก้ไขปัญหาการโหลดรูปใน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148418"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>แก้ไขปัญหาการโหลดรูปใน Yammer

เมื่อเกิดปัญหากับรูปถ่ายและแสดงตัวอย่างแฟ้มใน Yammer แก้ไขปัญหา โดยตรวจสอบว่า ปัญหาที่เกิดขึ้นสําหรับผู้ใช้ทั้งหมด ไม่ว่าจะเป็นบนอุปกรณ์มือถือ และถ้าเป็น reproducible เมื่ออัปโหลดสิ่งที่แนบ  

**ปัญหารูปภาพโปรไฟล์**  

ถ้าผู้ใช้ลงชื่อเข้าใช้ Yammer ผ่าน Microsoft 365 ผู้ใช้เหล่านั้นต้องเปลี่ยนโปรไฟล์รวมถึงรูปโปรไฟล์ของผู้ใช้ หากผู้ใช้ไม่ได้รับอนุญาตให้อัปเดตโปรไฟล์ผู้ดูแลระบบสามารถทําการอัปเดตสําหรับผู้ใช้ได้ สําหรับข้อมูลเพิ่มเติม ให้ดูที่[ดูและอัปเดตโปรไฟล์ของคุณใน Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)

สําหรับข้อมูลเกี่ยวกับการแก้ไขโปรไฟล์ รวมถึงรูปโปรไฟล์ ให้ดูที่[การเปลี่ยนโปรไฟล์ Yammer และการตั้งค่าของฉัน](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851) 

รูปภาพโปรไฟล์ที่อัปเดตจะซิงค์แตกต่างจากคุณลักษณะโปรไฟล์ ผู้ใช้ต้องลงชื่อเข้าใช้เพื่อเริ่มต้นการซิงค์รูปโปรไฟล์ สําหรับข้อมูล[ให้ดูที่ รูปภาพโปรไฟล์ผู้ใช้ที่ได้รับการปรับปรุงจาก Office 365 ไปยัง Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)

สําหรับข้อมูลเกี่ยวกับวงจรการใช้งานของผู้ใช้สําหรับ Yammer ให้ดูที่[จัดการผู้ใช้ Yammer ในวงจรการใช้งานของผู้ใช้จาก Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)  

สําหรับรายละเอียดเกี่ยวกับวิธีการทํางานของการซิงค์รูปภาพโปรไฟล์ใน Microsoft 365 ให้ดูที่[ข้อมูลเกี่ยวกับการทําข้อมูลโปรไฟล์รูปภาพให้ตรงกันใน Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)  

**ตัวอย่างเอกสารและปัญหารูปขนาดย่อของภาพ**  

เมื่อไฟล์หรือรูปภาพถูกโพสต์ไปยัง Yammer การแสดงตัวอย่างอาจไม่ปรากฏขึ้นเนื่องจาก: 

- แฟ้มเสียหายและไม่สามารถประมวลผลได้
- แฟ้มไม่ได้ถูกอัปโหลดเมื่อเร็ว ๆ นี้ไปยัง SharePoint แบบออนไลน์ หรือ Yammer มีข้อมูลเมตาที่ไม่ถูกต้องสําหรับเหตุผลอื่น ๆ
- URL ที่จําเป็นสําหรับการโหลดภาพตัวอย่างจะถูกบล็อก
- การแสดงตัวอย่างไฟล์ถูกลบโดยผู้ใช้ก่อนที่จะลงรายการบัญชี
- ปัญหาการบริการทําให้การแสดงตัวอย่างถูกสร้างขึ้น

**หมายเหตุ** ตัวอย่างลิงก์และอัปโหลดไฟล์อาจทํางานแตกต่างกัน ลิงก์ไปยังแฟ้มบนอินเทอร์เน็ตหรือการเชื่อมโยงที่จําเป็นต้องมีการรับรองความถูกต้องเพิ่มเติมอาจแสดงไม่ถูกต้อง

สําหรับข้อมูลเพิ่มเติม ให้ดูที่[การแนบไฟล์หรือรูปภาพลงในข้อความ Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf) 