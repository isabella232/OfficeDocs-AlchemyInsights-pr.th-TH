---
title: ดับเบิลคลิกไฟล์Officeไม่สามารถเปิดไฟล์ได้
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 519051ac0ffc11d2b17c14959464c1123654bef38d6e10efd252b4ff3d8bbc1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965120"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>ดับเบิลคลิกไฟล์Officeไม่สามารถเปิดไฟล์ได้

หลังจากดับเบิลคลิกOfficeไฟล์ของคุณ คุณอาจเห็นโปรแกรมเปิดแต่ไฟล์ไม่เปิดขึ้น หรือคุณอาจได้รับข้อผิดพลาด: "มีปัญหาในการส่งสั่งไปยังโปรแกรม" มีหลายสาเหตุดังนี้ แต่วิธีแก้ปัญหาที่พบบ่อยที่สุดสองวิธีคือ:

- จากExcelตรวจสอบให้แน่ใจว่าคุณไม่ได้เลือกตัวเลือก DDE แล้ว ตัวเลือกสามารถพบได้โดยการสร้างเวิร์กบุ๊กใหม่ แล้วเลือก ไฟล์ > บันทึก>**ขั้นสูง** ในส่วน **ทั่วไป** ให้ยกเลิกการเลือก ละเว้น **แอปพลิเคชันอื่นที่ใช้ การตั้งค่าExchange (DDE)**

- เรียกใช้ การซ่อมแซมแบบออนไลน์ เพื่อคืนค่าการตั้งค่าเริ่มต้น คลิกปุ่ม Windows เริ่ม แล้วค้นหา "แผงควบคุม" เปิด **แผงควบคุม แล้ว** ไปที่ โปรแกรม **> และ** ฟีเจอร์ จากนั้นคลิกขวาที่ Microsoft Office **[เวอร์ชัน]** แล้วเลือก **เปลี่ยน>ซ่อมแซม** แบบออนไลน์

ถ้าโซลูชันเหล่านี้ไม่ได้ผล คุณสามารถดูรายการโซลูชันทั้งหมดได้ในบทความสนับสนุน การดับเบิลคลิกไฟล์[Office ไม่สามารถเปิดไฟล์](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)ได้
