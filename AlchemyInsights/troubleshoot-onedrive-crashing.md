---
title: การแก้ไขปัญหาการหยุดทํางานของ OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749171"
---
# <a name="troubleshoot-onedrive-crashes"></a>การแก้ไขปัญหาการหยุดทํางานของ OneDrive

หาก OneDrive ล้มเหลวซ้ํา ๆ ลองทําตามขั้นตอนการแก้ไขปัญหาเหล่านี้:

**ตรวจสอบให้แน่ใจว่าไม่ได้ตั้งค่ารีจิสทรีคีย์:**

1. การใช้ตัวแก้ไขรีจิสทรี ให้นําทางไปยัง HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. ถ้า DisableFileSyncNGSC อยู่ และตั้งค่าเป็น 1 เปิดคีย์ และเปลี่ยนค่าเป็น 0
3. เปิดใช้ OneDrive ด้วยตนเองโดยไปที่หน้าจอเริ่ม ![กดแป้น Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)ประเภท:OneDriveในกล่องค้นหา แล้วคลิกบนแอป OneDrive เดสก์ท็อป

**รีเซ็ต OneDrive:**

หมาย เหตุ:

- การรีเซ็ต OneDrive จะยกเลิกการเชื่อมต่อการซิงค์ทั้งหมดที่มีอยู่ (รวมถึง OneDrive ส่วนบุคคลของคุณถ้าตั้งค่า)
- คุณจะไม่สูญเสียไฟล์หรือข้อมูลด้วยการรีเซ็ต OneDrive บนคอมพิวเตอร์ของคุณ

**เมื่อต้องการรีเซ็ต OneDrive:**

1. เปิดกล่องโต้ตอบเรียกใช้โดยการกดแป้น Windows และ R
2. พิมพ์ %localappdata%\Microsoft\OneDrive\onedrive.exe /reset และกด ตกลง หน้าต่างคําสั่งอาจปรากฏขึ้นสั้น ๆ
3. เปิดใช้ OneDrive ด้วยตนเองโดยไปที่หน้าจอเริ่ม ![กดแป้น Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)ประเภท:OneDriveในกล่องค้นหา แล้วคลิกบนแอป OneDrive เดสก์ท็อป

หมาย เหตุ:

- หากคุณเลือกที่จะซิงค์เฉพาะบางโฟลเดอร์ก่อนการตั้งค่าใหม่ คุณจะต้องทําอีกครั้งเมื่อซิงค์เสร็จสิ้น อ่าน [เลือกโฟลเดอร์ OneDrive ที่จะซิงค์กับคอมพิวเตอร์ของคุณ](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   สําหรับข้อมูลเพิ่มเติม
- คุณจะต้องดําเนินการนี้ให้เสร็จสมบูรณ์สําหรับ OneDrive ส่วนบุคคลของคุณและ OneDrive สําหรับธุรกิจ