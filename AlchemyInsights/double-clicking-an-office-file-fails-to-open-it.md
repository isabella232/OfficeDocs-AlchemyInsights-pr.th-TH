---
title: ดับเบิลคลิกไฟล์ Office เพื่อเปิดไม่สํานักงาน
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
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814824"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>ดับเบิลคลิกไฟล์ Office เพื่อเปิดไม่สํานักงาน

หลังจากดับเบิลคลิกที่ไฟล์ Office คุณอาจเห็นโปรแกรมเปิดแต่ไฟล์ไม่เปิดขึ้น หรือคุณอาจได้รับข้อผิดพลาด: "มีปัญหาในการส่งสั่งไปยังโปรแกรม" มีหลายสาเหตุดังนี้ แต่วิธีแก้ปัญหาที่พบบ่อยที่สุดสองวิธีคือ:

- จากภายใน Excel ตรวจสอบให้แน่ใจว่าไม่ได้เลือกตัวเลือก DDE แล้ว ตัวเลือกสามารถพบได้โดยการสร้างเวิร์กบุ๊กใหม่ แล้วเลือก ไฟล์ > บันทึก>**ขั้นสูง** ในส่วน **ทั่วไป** ให้ยกเลิกการเลือก **ละเว้นแอปพลิเคชันอื่นที่ใช้ Dynamic Data Exchange (DDE)**

- เรียกใช้ การซ่อมแซมแบบออนไลน์ เพื่อคืนค่าการตั้งค่าเริ่มต้น คลิกปุ่ม เริ่ม ของ Windows แล้วค้นหา "แผงควบคุม" เปิด **แผงควบคุม แล้ว** ไปที่ โปรแกรม **> และ** ฟีเจอร์ คลิกขวาที่ Microsoft **Office [เวอร์ชัน] แล้วเลือก** เปลี่ยน **>ซ่อมแซม** แบบออนไลน์

ถ้าโซลูชันเหล่านี้ไม่ได้ผล คุณสามารถดูรายการโซลูชันทั้งหมดได้ในบทความสนับสนุน ดับเบิล [คลิกไฟล์ Office ล้มเหลวในการ](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)เปิด
