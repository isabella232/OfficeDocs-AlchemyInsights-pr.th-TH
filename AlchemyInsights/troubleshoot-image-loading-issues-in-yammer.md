---
title: แก้ไขปัญหาการโหลดรูปภาพYammer
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
ms.openlocfilehash: 11315fd84f92251e435320f4550286fb2db4b0128f7ac85c0f79972e3f7fd203
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939254"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a>แก้ไขปัญหาการโหลดรูปภาพYammer

เมื่อเกิดปัญหากับรูปถ่ายและการแสดงตัวอย่างไฟล์ใน Yammer ให้แก้ไขปัญหาโดยการตรวจสอบว่าปัญหาจะเกิดขึ้นกับผู้ใช้ทั้งหมดหรือไม่ไม่ว่าจะเกิดขึ้นบนอุปกรณ์เคลื่อนที่หรือไม่ และถ้าเกิดปัญหานี้ขึ้นใหม่เมื่ออัปโหลดสิ่งที่แนบมา  

**ปัญหารูปภาพโปรไฟล์**  

ถ้าผู้ใช้ลงชื่อเข้าใช้Yammerผ่านทาง Microsoft 365พวกเขาต้องเปลี่ยนโปรไฟล์ของพวกเขา รวมถึงรูปภาพโปรไฟล์ของพวกเขา If users are not permitted to make profile updates, an admin can make the update for the user. ดูข้อมูลเพิ่มเติมได้ที่ ดู[และอัปเดตโปรไฟล์Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)

For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851). 

รูปถ่ายโปรไฟล์ที่อัปเดตจะซิงค์แตกต่างจากแอตทริบิวต์โปรไฟล์ ผู้ใช้ต้องลงชื่อเข้าใช้เพื่อเริ่มต้นการซิงค์รูปภาพโปรไฟล์ของพวกเขา For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).

For info about the user lifecycle for Yammer, [see Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).  

For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).  

**ตัวอย่างเอกสารและปัญหารูปขนาดย่อ**  

เมื่อไฟล์หรือรูปภาพถูกโพสต์Yammer การแสดงตัวอย่างอาจไม่ปรากฏขึ้นเนื่องจาก: 

- ไฟล์เสียหายและไม่สามารถประมวลผลได้
- ไฟล์ยังไม่ถูกอัปโหลดไปยังไฟล์ SharePoint Online หรือ Metadata Yammerเมตาดาต้าไม่ถูกต้องด้วยเหตุผลอื่นๆ
- URL ที่ต้องใช้ในการโหลดรูปภาพตัวอย่างจะถูกบล็อก
- ผู้ใช้ก่อนที่จะโพสต์การแสดงตัวอย่างไฟล์จะถูกเอาออก
- ปัญหาบริการป้องกันไม่ให้มีการสร้างการแสดงตัวอย่าง

**หมายเหตุ** การแสดงตัวอย่างของลิงก์และการอัปโหลดไฟล์อาจมีลักษณะการอัปโหลดต่างกัน ลิงก์ไปยังไฟล์บนอินเทอร์เน็ตหรือลิงก์ที่ต้องมีการรับรองความถูกต้องเพิ่มเติมอาจแสดงไม่ถูกต้อง

หากต้องการข้อมูลเพิ่มเติม โปรดดู[แนบไฟล์หรือรูปYammerข้อความ](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf) 