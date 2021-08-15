---
title: ปัญหากับผู้ใช้รายเดียว
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
- "8469"
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960170"
---
# <a name="problem-with-single-user"></a>ปัญหากับผู้ใช้รายเดียว

- ผู้ใช้อาจยังไม่ได้เตรียมใช้งานเนื่องจากบริการยังไม่มีโอกาสที่จะประเมินผู้ใช้ ตรวจสอบแนวทางสําหรับระยะเวลาที่การเตรียมใช้งานและแถบความคืบหน้าบนหน้าการกําหนดค่าการเตรียมใช้งาน ถ้าสถานะคงที่ที่ระบุไว้ในส่วนรายละเอียดเพิ่มเติมอยู่ก่อนวันที่ผู้ใช้ถูกสร้าง/อัปเดต/ลบ หมายความว่าเรายังไม่ได้ประเมินผู้ใช้ ในสถานการณ์นี้ วิธีที่ดีที่สุดคือรอให้บริการการเตรียมใช้งานเสร็จสิ้น

  - โปรดทราบว่าบริการของเราจะทราบถึงการเปลี่ยนแปลงของผู้ใช้ในระบบต้นทางเท่านั้น (Cloud HR) มีการเปลี่ยนแปลงที่ถูกต้องในระบบต้นทางของ Azure AD เพื่อตรวจหาการเปลี่ยนแปลงและโฟลว์ลงใน Active Directory
- บริการการเตรียมใช้งานประเมินผู้ใช้และกําหนดว่าไม่ควรเตรียมใช้งาน:
  - ถ้าคุณได้ตั้งค่าตัวกรองการใส่ช่วงแอตทริบิวต์ ตรวจสอบให้แน่ใจว่าผู้ใช้ตรงตามเกณฑ์ที่คุณระบุ
  - If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.
- บริการการเตรียมใช้งานพยายามเตรียมใช้งานผู้ใช้ แต่ล้มเหลว For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:
  - แอตทริบิวต์ที่ต้องมีในผู้ใช้อาจหายไปใน Active Directory ภายในองค์กรหรือ Azure AD ตัวอย่างเช่น กฎ userPrincipalName หรือ sAMAccountName Generation ไม่ได้สร้างค่าที่ถูกต้อง
  - แอตทริบิวต์ที่ตรงกัน (มักจะเป็น employeeId) ไม่แก้ไขให้ผู้ใช้ที่ไม่ซ้้ากันใน Active Directory ภายในองค์กรหรือ Azure AD ตัวอย่างเช่น มีผู้ใช้สองคนที่มี employeeId เดียวกันใน AD และบริการส่งกลับรหัสข้อผิดพลาดจะระบุรายการเป้าหมายที่คัดลอกกันของรายการแหล่งข้อมูลเดียวกัน

เมื่อต้องการรีวิวบันทึกของผู้ใช้และกลุ่มเดียว ให้ดู[ตรวจทานบันทึกการเตรียมใช้งานเพื่อแก้ไขปัญหากับผู้ใช้ที่ระบุ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
