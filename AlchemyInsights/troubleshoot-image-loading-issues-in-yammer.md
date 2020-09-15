---
title: การแก้ไขปัญหาการโหลดรูปภาพใน Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: cf330adbf3f3a92d4b90768c7dd8bada6333db80
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690262"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>การแก้ไขปัญหาการโหลดรูปภาพใน Yammer

เมื่อปัญหาเกิดขึ้นกับรูปถ่ายและการแสดงตัวอย่างไฟล์ใน Yammer การแก้ไขปัญหาโดยการตรวจสอบว่าปัญหานี้เกิดขึ้นสำหรับผู้ใช้ทั้งหมดหรือไม่ไม่ว่าจะเกิดปัญหาในอุปกรณ์เคลื่อนที่และถ้าการอัปโหลดสิ่งที่แนบมา  

**ปัญหารูปถ่ายของโพรไฟล์**  

ถ้าผู้ใช้ลงชื่อเข้าใช้ Yammer ผ่าน Microsoft ๓๖๕ผู้ใช้จะต้องเปลี่ยนโปรไฟล์ของพวกเขารวมถึงรูปภาพโปรไฟล์ของพวกเขา ถ้าผู้ใช้ไม่ได้รับอนุญาตให้ทำการอัปเดตโปรไฟล์ผู้ดูแลระบบสามารถทำการอัปเดตสำหรับผู้ใช้ได้ สำหรับข้อมูลเพิ่มเติมให้ดูที่[ดูและอัปเดตโปรไฟล์ของคุณใน Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)

สำหรับข้อมูลเกี่ยวกับการแก้ไขส่วนกำหนดค่ารวมถึงรูปถ่ายโปรไฟล์ให้ดูที่[เปลี่ยนโปรไฟล์ Yammer และการตั้งค่าของฉัน](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851) 

รูปถ่ายโปรไฟล์ที่อัปเดตจะซิงค์แตกต่างจากแอตทริบิวต์โปรไฟล์ ผู้ใช้ต้องลงชื่อเข้าใช้เพื่อเริ่มการซิงค์รูปถ่ายโปรไฟล์ของพวกเขา สำหรับข้อมูลให้ดู[ที่รูปภาพโปรไฟล์ผู้ใช้ได้รับการอัปเดตจาก Office ๓๖๕ไปยัง Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer)

สำหรับข้อมูลเกี่ยวกับวงจรการใช้งานของผู้ใช้สำหรับ Yammer ให้ดูที่[จัดการผู้ใช้ Yammer ในวงจรชีวิตของพวกเขาจาก Office ๓๖๕](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle)  

สำหรับรายละเอียดเกี่ยวกับวิธีการซิงค์รูปภาพโปรไฟล์ทำงานใน Microsoft ๓๖๕ให้ดูที่[ข้อมูลเกี่ยวกับการซิงโครไนซ์รูปภาพโปรไฟล์ใน microsoft ๓๖๕](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a)  

**การแสดงตัวอย่างเอกสารและปัญหารูปขนาดย่อของรูป**  

เมื่อมีการโพสต์ไฟล์หรือรูปภาพไปยัง Yammer การแสดงตัวอย่างอาจไม่ปรากฏขึ้นเนื่องจาก: 

- ไฟล์เสียหายและไม่สามารถประมวลผลได้
- ไฟล์นี้ยังไม่ได้รับการอัปโหลดไปยัง SharePoint Online หรือ Yammer มี metadata ที่ไม่ถูกต้องสำหรับเหตุผลอื่นๆ
- Url ที่จำเป็นสำหรับการโหลดรูปภาพตัวอย่างจะถูกบล็อก
- การแสดงตัวอย่างไฟล์ถูกเอาออกโดยผู้ใช้ก่อนที่จะลงรายการบัญชี
- ปัญหาของบริการที่ทำให้การแสดงตัวอย่างถูกสร้างขึ้น

**หมายเหตุ:** การแสดงตัวอย่างสำหรับลิงก์และการอัปโหลดไฟล์อาจทำงานแตกต่างกัน ลิงก์ไปยังไฟล์บนอินเทอร์เน็ตหรือลิงก์ที่จำเป็นต้องมีการรับรองความถูกต้องเพิ่มเติมอาจแสดงไม่ถูกต้อง

สำหรับข้อมูลเพิ่มเติมให้ดู[ที่แนบไฟล์หรือรูปภาพไปยังข้อความ Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf) 