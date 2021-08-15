---
title: การกําหนดค่าบริการการเตรียมใช้งาน
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
ms.openlocfilehash: 271ab7ad34c0f85f6f5a9d8d3dc2d901fe6fe8f978a2cc98eed986f594036f17
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033297"
---
# <a name="configuring-the-provision-service"></a>การกําหนดค่าบริการการเตรียมใช้งาน

เพื่อให้การเตรียมใช้งานผู้ใช้ที่ใช้งานได้โดยอัตโนมัติ Azure AD ต้องใช้ข้อมูลรับรองที่ถูกต้องที่อนุญาตให้เชื่อมต่อกับ API ของบริการเว็บ Workday นอกจากนี้ปุ่มทดสอบการเชื่อมต่อในวันการเตรียมใช้งานผู้ใช้ AD ยังตรวจสอบว่าสามารถเชื่อมต่อกับ Azure AD เชื่อมต่อตัวแทนการเตรียมใช้งานที่เชื่อมโยงกับโดเมน AD หรือไม่

ถ้าพอร์ทัล Azure ส่งกลับข้อผิดพลาดเมื่อบันทึกข้อมูลอ้างอิง ให้ปฏิบัติตามขั้นตอนที่แนะนาทางด้านล่าง:

1. ยืนยันว่าคุณได้กําหนดค่าบัญชีผู้ใช้ระบบการรวมของวันงานตามที่ระบุไว้ในส่วนบทช่วยสอน[กําหนดค่าผู้ใช้ระบบการรวมใน Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)
2. ยืนยันว่าบริการตัวแทนเชื่อมต่อ Azure AD เริ่มต้นและเรียกใช้งานบนเซิร์ฟเวอร์Windowsภายในองค์กรของคุณโดยใช้คอนโซลการจัดการบริการ คุณยังสามารถตรวจสอบสถานะของตัวแทนในพอร์ทัล Azure โดยการคลิกปุ่ม ดูตัวแทนภายในองค์กร
3. ตรวจสอบให้แน่ใจว่าคุณใส่ค่าเขตข้อมูล "ชื่อผู้ใช้ของวันงาน" โดยใช้รูปแบบusername@workday-tenant-name ถ้า workday-tenant-name หายไป การรับรองความถูกต้องของ Workday ล้มเหลว
4. ถ้าคุณกําหนดค่าการรวมกับผู้เช่าการปรับใช้วันงาน ให้สังเกตชั่วโมงการหยุดใช้งานที่กําหนดไว้ของผู้เช่า Workday ของคุณ วันงานได้จัดเวลาหยุดให้บริการผู้เช่าในช่วงวันหยุดสุดสัปดาห์ (โดยปกติจะเป็นช่วงเย็นวันศุกร์ถึงเช้าวันเสาร์) และความล้มเหลวในการเชื่อมต่อระหว่างหน้าต่างการหยุดให้บริการนี้เป็นปัญหาที่ทราบแล้วซึ่งการแก้ไขโดยอัตโนมัติทันทีที่ผู้เช่าการปรับใช้กลับมาออนไลน์
5. ในบางกรณี คุณอาจเห็นข้อผิดพลาดนี้ถ้ารหัสผ่านของผู้ใช้ Integration System เปลี่ยนแปลงไปเนื่องจากการรีเฟรชผู้เช่า หรือถ้าบัญชีอยู่ในสถานะล็อกหรือหมดอายุ โปรดตรวจสอบสถานะของผู้ใช้ระบบการรวมกับผู้ดูแลระบบของวันการงานของคุณ

For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).
