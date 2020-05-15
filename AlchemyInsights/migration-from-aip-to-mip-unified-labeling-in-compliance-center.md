---
title: การย้ายข้อมูลจาก AIP ไปยังการติดป้ายชื่อ MIP/รวมในศูนย์การปฏิบัติตามกฎระเบียบ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7ce9c387fc94f59674a922c5fe071fc0fb030344
ms.sourcegitcommit: e6d73d240669342fde9d4d25b0ee2838b7e43965
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 05/14/2020
ms.locfileid: "44236566"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>การย้ายข้อมูลจาก AIP ไปยังการติดป้ายชื่อ MIP/รวมในศูนย์การปฏิบัติตามกฎระเบียบ

เมื่อต้องการโยกย้ายจากป้ายชื่อ AIP ไปยัง Unified Labeling ในศูนย์ความปลอดภัยและการปฏิบัติตามกฎระเบียบ ให้ทําดังนี้

**เปิดใช้งานการป้องกันจากพอร์ทัล Azure**

1. ถ้าคุณยังไม่ได้ทํา ให้เปิดหน้าต่างเบราว์เซอร์ใหม่แล้ว[ลงชื่อเข้าใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) นําทางไปยังใบ**ป้องกันข้อมูล Azure** ตัวอย่างเช่น บนเมนูฮับ คลิก**บริการทั้งหมด**และเริ่มพิมพ์**ข้อมูล**ในกล่องตัวกรอง เลือก**การป้องกันข้อมูล Azure** ถ้าคุณยังไม่ได้เข้าถึงใบป้องกันข้อมูล Azure ก่อน ดู[ขั้นตอนเพิ่มเติม](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)แบบครั้งเดียวเพื่อเพิ่มใบนี้ไปยังพอร์ทัล เมื่อต้องการเปิดใบป้องกันข้อมูล Azure คุณต้องมี[แผน Azure ป้องกันข้อมูลแบบพิเศษ](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing)หรือแผน Office 365 ที่มีการจัดการสิทธิ์ ถ้าคุณมีการสมัครใช้งานเหล่านี้แต่เห็นข้อความว่าไม่พบการสมัครใช้งานที่ถูกต้อง[โปรดติดต่อฝ่ายสนับสนุนของ Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support)หรือใช้ช่องทางการสนับสนุนมาตรฐานของคุณ

2. ค้นหาตัวเลือก**เมนูจัดการ**และเลือก**การเปิดใช้งานการป้องกัน** คลิก**เปิดใช้งาน**แล้วยืนยันการดําเนินการของคุณ เมื่อเปิดใช้งานเสร็จสมบูรณ์**Activation finished successfully**

**โยกย้ายป้ายชื่อการป้องกันข้อมูล Azure ไปยังศูนย์การปฏิบัติตามข้อกําหนด&ความปลอดภัยของ Office 365**

1. ตรวจสอบให้แน่ใจว่า คุณได้เข้าสู่ระบบในฐานะผู้ใช้ที่มีสิทธิ์ของผู้ดูแลระบบส่วนกลาง

2. นําทางไปยังใบ**ป้องกันข้อมูล Azure**

3. จากตัวเลือก**จัดการ**เมนู ให้เลือก**การติดป้ายชื่อแบบรวม**

4. บน**การป้องกันข้อมูล Azure - ใบติดฉลากแบบรวม**คลิก**เปิดใช้งาน**และทําตามคําแนะนําแบบออนไลน์

**หมายเหตุ**: ตรวจสอบว่า คุณมีสิทธิ์ที่เหมาะสมก่อนที่จะเปิดใช้งานการรักษาความปลอดภัย&ศูนย์ปฏิบัติตามกฎระเบียบการโยกย้าย ดูบทความเหล่านี้สําหรับข้อมูลเพิ่มเติม:

1. [คุณต้องเป็นผู้ดูแลระบบส่วนกลางเพื่อกําหนดค่าการป้องกันข้อมูล Azure หรือฉันสามารถมอบสิทธิ์ให้กับผู้ดูแลระบบอื่นได้หรือไม่](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [ข้อมูลสําคัญเกี่ยวกับบทบาทการดูแลระบบหลังจากโยกย้ายไปยังศูนย์การปฏิบัติตามกฎระเบียบ&ความปลอดภัย](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับ AIP ไปยังการโยกย้ายการติดฉลากแบบรวมไปยังความปลอดภัยและศูนย์การปฏิบัติตามกฎระเบียบ ให้ดูที่[โยกย้ายป้ายชื่อ](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
