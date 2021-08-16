---
title: การโยกย้ายจาก AIP ไปยังป้ายชื่อ MIP/Unified ในศูนย์การปฏิบัติตามข้อบังคับ
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
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000385"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>การโยกย้ายจาก AIP ไปยังป้ายชื่อ MIP/Unified ในศูนย์การปฏิบัติตามข้อบังคับ

เมื่อต้องการโยกย้ายจากป้ายชื่อ AIP ไปยังป้ายชื่อแบบครบวงจรในศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย ให้ปฏิบัติดังนี้

**เปิดใช้งานการป้องกันจากพอร์ทัล Azure**

1. ถ้าคุณยังไม่ได้เปิด ให้เปิดหน้าต่างเบราว์เซอร์ใหม่และ[ลงชื่อเข้าใช้พอร์ทัล Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) นําทางไปยัง **เบลด Azure Information Protection** ตัวอย่างเช่น บนเมนูฮับ ให้คลิก **บริการทั้งหมด** แล้วเริ่ม **พิมพ์** ข้อมูล ในกล่อง ตัวกรอง เลือก **Azure Information Protection** ถ้าคุณไม่เคยเข้าถึงเบลด Azure Information Protection มาก่อน ให้ดูขั้นตอนเพิ่มเติมแบบใช้ [เวลา](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) เดียวเพื่อเพิ่มเบลดนี้ลงในพอร์ทัล เมื่อต้องการเปิดเบลด Azure Information Protection คุณต้องมีแผน[Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing)หรือแผนการจัดการOffice 365ที่มีการจัดการสิทธิ์ ถ้าคุณมีหนึ่งในการสมัครใช้งานเหล่านี้ แต่เห็นข้อความว่าไม่พบการสมัครใช้งานที่ถูกต้อง ติดต่อฝ่ายสนับสนุนของ [Microsoft หรือใช้](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) แชนเนลการสนับสนุนมาตรฐานของคุณ

2. ค้นหา **ตัวเลือก** เมนู จัดการ แล้วเลือก **การเปิดใช้งาน** การป้องกัน คลิก **เปิดใช้งาน** แล้วยืนยันการทํางานของคุณ เมื่อเปิดใช้งานเสร็จสมบูรณ์ แถบข้อมูลจะแสดง การเปิดใช้งาน **เสร็จสมบูรณ์**

**โยกย้ายป้ายชื่อ Azure Information Protection ไปยังศูนย์Office 365การรักษา&นโยบาย**

1. ตรวจสอบให้แน่ใจว่าคุณเข้าสู่ระบบในฐานะผู้ใช้ที่มีสิทธิ์ผู้ดูแลระบบส่วนกลาง

2. นําทางไปยัง **เบลด Azure Information Protection**

3. จาก **ตัวเลือก** เมนูจัดการ **ให้เลือก การติดป้ายผนึก** แบบรวม

4. บน **Azure Information Protection - ใบป้ายชื่อแบบรวม** ให้คลิก **เปิดใช้งาน และ** ปฏิบัติตามคําแนะนําแบบออนไลน์

**หมายเหตุ**: ตรวจสอบว่าคุณมีสิทธิ์ที่เหมาะสมก่อนที่จะเปิดใช้งานการโยกย้ายศูนย์&การปฏิบัติตามนโยบาย ดูบทความเหล่านี้เพื่อดูข้อมูลเพิ่มเติม:

1. [คุณต้องเป็นผู้ดูแลระบบส่วนกลางเพื่อกําหนดค่า Azure Information Protection หรือฉันสามารถมอบสิทธิ์ให้กับผู้ดูแลระบบคนอื่นได้หรือไม่](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [ข้อมูลสําคัญเกี่ยวกับบทบาทผู้ดูแลระบบหลังจากการโยกย้ายไปยังศูนย์&การปฏิบัติตามนโยบาย](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
