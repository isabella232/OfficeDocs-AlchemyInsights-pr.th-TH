---
title: ส่งข้อความอีเมลด้วยการให้ ID ข้อความเครือข่าย
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695379"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a>ส่งข้อความอีเมลด้วยการให้ ID ข้อความเครือข่าย

1. ใน **แถบปลิว** การส่งใหม่ **ให้เลือกอีเมล****และ ID ข้อความ** เครือข่าย
2. ให้ปฏิบัติตามขั้นตอนเหล่านี้เพื่อค้นหา ID ข้อความของข้อความอีเมลใน Outlook:
    1. ดับเบิลคลิกที่ข้อความอีเมลเพื่อเปิด
    1. **เลือก**  >  **คุณสมบัติ** ไฟล์
    1. เปิด Notepad หรือเอกสาร Word เปล่า แล้วคัดลอกและวางเนื้อหาที่พบในกล่อง **ส่วนหัวอินเทอร์เน็ต** ลงในเอกสารที่เปิดอยู่เพื่อให้มองเห็นได้ดียิ่งขึ้น
    1. ค้นหาเขตข้อมูล **X-MS-Exchange-Organization-Network-Message-Id** ค่าหลังจาก **:** คือ ID ที่คุณต้องการส่ง
3. **ภายใต้ ผู้รับ** ถ้าอีเมลอยู่ในโฟลเดอร์อีเมลขยะของผู้รับอีเมลนี้ทั้งหมด ให้เลือก **เลือก** ทั้งหมด ถ้าไม่ ให้เลือกเฉพาะผู้ใช้ที่รายงานปัญหา
4. ภายใต้ **เหตุผล** ในการส่ง ถ้าคุณเลือกควรถูกบล็อก ให้ระบุว่าข้อความควรถูกบล็อกเป็น **สแปม** ฟิชชิ่ง หรือมัลแวร์ จากนั้นเลือกส่ง

เมื่อต้องการเรียนรู้เพิ่มเติม[ให้ดูวิธีการส่งสแปมที่น่าสงสัย, phish, URL และไฟล์ไปยัง Microsoft เพื่อสแกน](https://go.microsoft.com/fwlink/?linkid=2101479)
