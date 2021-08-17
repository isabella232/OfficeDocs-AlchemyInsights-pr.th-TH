---
title: ค้นหาเหตุการณ์ที่ปฏิบัติตามกฎกล่องจดหมายเข้า
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882654"
---
# <a name="find-events-performed-on-inbox-rules"></a>ค้นหาเหตุการณ์ที่ปฏิบัติตามกฎกล่องจดหมายเข้า

เมื่อกฎกล่องจดหมายเข้าถูกสร้าง เปลี่ยนแปลง หรือลบ เหตุการณ์จะถูกบันทึกในบันทึกการตรวจสอบ ต่อไปนี้เป็นวิธีตรวจสอบ:

1. เลือกเลือกอย่างใดอย่างหนึ่งต่อไปนี้
   - ในศูนย์การปฏิบัติตามข้อบังคับสําหรับ Microsoft 365 ที่ ให้ไปที่ <https://compliance.microsoft.com>  \> **ตรวจสอบโซลูชัน** หรือ เมื่อต้องการไปยัง **หน้า ตรวจสอบ** <https://compliance.microsoft.com/auditlogsearch> โดยตรง ให้ใช้
   - ในMicrosoft 365 Defenderที่ <https://security.microsoft.com> **ให้ไปที่** ตรวจสอบ หรือ เมื่อต้องการไปยัง **หน้า ตรวจสอบ** <https://security.microsoft.com/auditlogsearch> โดยตรง ให้ใช้

    > [!NOTE]
    > ถ้าคุณเห็นการแจ้งเตือนว่าคุณต้องเปิดการตรวจสอบ ให้เดินหน้าแล้วเปิดในตอนนี้ ถ้าไม่ได้เปิดฟีเจอร์นี้ ผลลัพธ์การค้นหาจะไม่สามารถดึงข้อมูลจากวันที่ก่อนหน้าได้

2. บนแท็บ **ค้นหา** ของหน้า **ตรวจสอบ** ให้กําหนดค่าการตั้งค่าต่อไปนี้
   - **ช่วงวันที่และเวลา**: เลือกช่วงวันที่/เวลา **ในกล่อง** เริ่มต้น **และ** สิ้นสุด
   - **กิจกรรม**: เลือก **กฎกล่องจดหมายเข้าใหม่ สร้างกฎกล่องจดหมายเข้าOutlook Web App**

3. เมื่อคุณเสร็จสิ้น **ให้คลิก** ค้นหา กิจกรรมจะปรากฏในหน้า **การค้นหาการตรวจสอบ** ใหม่

4. เลือกกิจกรรมในผลลัพธ์เพื่อเปิดเมนูปลิวรายละเอียด ภายใต้ **ส่วน** พารามิเตอร์ คุณสามารถดูชื่อของกฎ ชุดเงื่อนไข และการแอคชันที่กฎนั้นจะได้รับ

เมื่อต้องการเรียนรู้เพิ่มเติม [ให้ดู ค้นหาบันทึกการตรวจสอบเพื่อตรวจสอบปัญหาการสนับสนุน](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)ทั่วไป
