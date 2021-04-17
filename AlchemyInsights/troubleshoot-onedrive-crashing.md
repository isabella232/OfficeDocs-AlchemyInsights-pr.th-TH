---
title: แก้ไขปัญหาการหยุดการหยุดการ OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826218"
---
# <a name="troubleshoot-onedrive-crashes"></a>แก้ไขปัญหาการหยุดการหยุดการ OneDrive

ถ้า OneDrive หยุดการเกิดขึ้นซ้ําๆ ให้ลองขั้นตอนการแก้ไขปัญหาเหล่านี้:

**ตรวจสอบให้แน่ใจว่าไม่ได้ตั้งค่ารีจิสทรีคีย์:**

1. ใช้ Registry Editor นําทางHKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. ถ้า DisableFileSyncNGSC แสดงอยู่และตั้งค่าเป็น 1 ให้เปิดคีย์และเปลี่ยนค่าเป็น 0
3. เปิดใช้ OneDrive ด้วยตนเอง โดยไปที่เริ่ม ![กดแป้น Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)พิมพ์ OneDrive ในกล่องค้นหา แล้วคลิกแอป OneDrive บนเดสก์ท็อป

**รีเซ็ต OneDrive:**

หมายเหตุ:

- การรีเซ็ต OneDrive จะยกเลิกการเชื่อมต่อการซิงค์ที่มีอยู่ของคุณทั้งหมด (รวมถึง OneDrive ส่วนบุคคลของคุณถ้าตั้งค่าไว้)
- คุณจะไม่สูญเสียไฟล์หรือข้อมูลโดยการรีเซ็ต OneDrive บนคอมพิวเตอร์ของคุณ

**เมื่อต้องการรีเซ็ต OneDrive:**

1. เปิดกล่องโต้ตอบ เรียกใช้ โดยการกดแป้น Windows และ R
2. พิมพ์ %localappdata%\Microsoft\OneDrive\onedrive.exe /reset แล้วกด ตกลง หน้าต่าง Command อาจปรากฏขึ้นสั้นๆ
3. เปิดใช้ OneDrive ด้วยตนเอง โดยไปที่เริ่ม ![กดแป้น Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)พิมพ์ OneDrive ในกล่องค้นหา แล้วคลิกแอป OneDrive บนเดสก์ท็อป

หมายเหตุ:

- ถ้าคุณเลือกที่จะซิงค์เฉพาะบางโฟลเดอร์ก่อนการรีเซ็ต คุณจะต้องซิงค์อีกครั้งเมื่อการซิงค์เสร็จสมบูรณ์ อ่าน [เลือกโฟลเดอร์ OneDrive ที่คุณต้องการซิงค์กับคอมพิวเตอร์](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   ของคุณ เพื่อดูข้อมูลเพิ่มเติม
- คุณจะต้องเสร็จสิ้นการนี้กับ OneDrive ส่วนบุคคลของคุณและ OneDrive for Business