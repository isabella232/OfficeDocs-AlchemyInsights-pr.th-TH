---
title: การกําหนดค่าบริการเตรียมใช้งาน
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484046"
---
# <a name="configuring-the-provision-service"></a>การกําหนดค่าบริการเตรียมใช้งาน

เพื่อให้การเตรียมใช้งานผู้ใช้โดยอัตโนมัติใช้งานได้ Azure AD ต้องการข้อมูลรับรองที่ถูกต้องที่อนุญาตให้เชื่อมต่อกับ API ของบริการเว็บของ Workday นอกจากนี้ ปุ่มทดสอบการเชื่อมต่อบนวันการเตรียมใช้งานผู้ใช้ AD ยังตรวจสอบความถูกต้องถ้าสามารถเชื่อมต่อกับ Azure AD Connect Provisioning Agent ที่เชื่อมโยงกับโดเมน AD

ถ้าพอร์ทัล Azure ส่งกลับข้อผิดพลาดเมื่อบันทึกข้อมูลอ้างอิง ให้ปฏิบัติตามขั้นตอนที่แนะนาทางด้านล่าง:

1. ยืนยันว่าคุณได้กําหนดค่าบัญชีผู้ใช้ระบบการรวมของวันงานตามที่ระบุไว้ในส่วนบทช่วยสอน กําหนดค่า[ผู้ใช้ระบบการรวมใน Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. ยืนยันว่า Azure AD Connect Provisioning Agent Service เปิดใช้งานอยู่และใช้งานบนเซิร์ฟเวอร์ Windows ภายในองค์กรของคุณโดยใช้คอนโซลการจัดการบริการ คุณยังสามารถตรวจสอบสถานะของตัวแทนในพอร์ทัล Azure โดยการคลิกปุ่มดูตัวแทนภายในองค์กร
3. ตรวจสอบให้แน่ใจว่าคุณใส่ค่าเขตข้อมูล "ชื่อผู้ใช้งาน" โดยใช้รูปแบบusername@workday-ผู้เช่า ถ้าชื่อผู้เช่าวันงานหายไป การรับรองความถูกต้องวันงานล้มเหลว
4. ถ้าคุณกําหนดค่าการรวมกับผู้เช่าการใช้งานวันงาน ให้สังเกตชั่วโมงการหยุดใช้งานที่กําหนดไว้ของผู้เช่าวันงานของคุณ วันงานได้จัดเวลาหยุดให้บริการผู้เช่าในช่วงวันหยุดสุดสัปดาห์ (โดยปกติคือช่วงเย็นวันศุกร์ถึงเช้าวันเสาร์) และความล้มเหลวในการเชื่อมต่อระหว่างหน้าต่างการหยุดให้บริการนี้เป็นปัญหาที่ทราบแล้วซึ่งแก้ไขโดยอัตโนมัติทันทีที่ผู้เช่าการปรับใช้กลับมาออนไลน์
5. ในบางกรณี คุณอาจเห็นข้อผิดพลาดนี้ถ้ารหัสผ่านของผู้ใช้ Integration System เปลี่ยนแปลงไปเนื่องจากการรีเฟรชผู้เช่า หรือถ้าบัญชีอยู่ในสถานะถูกล็อกหรือหมดอายุ โปรดตรวจสอบสถานะของผู้ใช้ระบบการรวมกับผู้ดูแลระบบของวันการงานของคุณ

For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
