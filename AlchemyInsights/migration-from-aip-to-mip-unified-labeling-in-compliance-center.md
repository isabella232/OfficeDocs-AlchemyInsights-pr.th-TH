---
title: การโยกย้ายจาก AIP ไปยัง MIP/Unified การติดป้ายในศูนย์การปฏิบัติตามนโยบาย
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674345"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>การโยกย้ายจาก AIP ไปยัง MIP/Unified การติดป้ายในศูนย์การปฏิบัติตามนโยบาย

เมื่อต้องการโยกย้ายจากป้ายชื่อ AIP เพื่อรวมการติดป้ายในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายให้ทำดังต่อไปนี้:

**เปิดใช้งานการป้องกันจากพอร์ทัล Azure**

1. ถ้าคุณยังไม่ได้ทำให้เปิดหน้าต่างเบราว์เซอร์ใหม่และ[ลงชื่อเข้าใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) นำทางไปยังใบมีด**การป้องกันข้อมูลของ Azure** ตัวอย่างเช่นบนเมนูฮับให้คลิก **บริการทั้งหมด** แล้วเริ่มพิมพ์ **ข้อมูล** ในกล่องตัวกรอง เลือก**การป้องกันข้อมูล Azure** ถ้าคุณยังไม่ได้เข้าถึงใบมีดการป้องกันข้อมูลของ Azure ก่อนให้ดู [ขั้นตอนเพิ่มเติม](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) แบบครั้งเดียวเพื่อเพิ่มใบมีดนี้ไปยังพอร์ทัล เมื่อต้องการเปิดใบมีดการป้องกันข้อมูลของ Azure คุณต้องมี [แผนพรีเมียมการป้องกันข้อมูลของ azure](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) หรือแผน Office ๓๖๕ที่มีการจัดการสิทธิ์ ถ้าคุณมีหนึ่งในการสมัครใช้งานเหล่านี้แต่เห็นข้อความว่าไม่พบการสมัครใช้งานที่ถูกต้องให้ [ติดต่อฝ่ายสนับสนุนของไมโครซอฟท์](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) หรือใช้ช่องทางการสนับสนุนมาตรฐานของคุณ

2. ค้นหาตัวเลือก**จัดการ**เมนูแล้วเลือก**การเปิดใช้งานการป้องกัน** คลิก **เปิดใช้งาน**แล้วยืนยันการดำเนินการของคุณ เมื่อการเปิดใช้งานเสร็จสมบูรณ์แล้วแถบข้อมูลจะแสดงการ**เปิดใช้งานเสร็จเรียบร้อยแล้ว**

**โยกย้ายป้ายชื่อการป้องกันข้อมูล Azure ไปยังศูนย์การรักษาความปลอดภัยของ Office ๓๖๕ & ศูนย์การปฏิบัติตามนโยบาย**

1. ตรวจสอบให้แน่ใจว่าคุณได้เข้าสู่ระบบในฐานะผู้ใช้ที่มีสิทธิ์ระดับผู้ดูแลระบบส่วนกลาง

2. นำทางไปยังใบมีด**การป้องกันข้อมูลของ Azure**

3. จากตัวเลือก**จัดการ**เมนูให้เลือกการ**ติดป้ายแบบครบวงจร**

4. บนหน้าการ **ป้องกันข้อมูลของ Azure-การติดป้ายชื่อแบบ** รวมให้คลิก **เปิดใช้งาน** แล้วทำตามคำแนะนำออนไลน์

**หมายเหตุ**: ตรวจสอบว่าคุณมีสิทธิ์ที่เหมาะสมก่อนที่จะเปิดใช้งานการโยกย้ายศูนย์การรักษาความปลอดภัย & การปฏิบัติตามนโยบาย ดูบทความเหล่านี้สำหรับข้อมูลเพิ่มเติม:

1. [คุณจำเป็นต้องเป็นผู้ดูแลระบบส่วนกลางเพื่อกำหนดค่าการป้องกันข้อมูลของ Azure หรือฉันสามารถมอบสิทธิ์ให้กับผู้ดูแลระบบรายอื่นได้หรือไม่](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [ข้อมูลที่สำคัญเกี่ยวกับบทบาทการดูแลระบบหลังจากโยกย้ายไปยังศูนย์การปฏิบัติตามกฎระเบียบ & ด้านความปลอดภัย](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับ AIP เพื่อรวมการโยกย้ายการโยกย้ายไปยังศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายให้ดูที่การ[โยกย้ายป้ายชื่อ](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
