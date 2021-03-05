---
title: การกําหนดค่าบริการการซิงค์ MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482895"
---
# <a name="configure-mim-sync-service"></a>การกําหนดค่าบริการการซิงค์ MIM

บริการการซิงโครไนซ์ Microsoft Identity Manager (MIM) เป็นคอมโพเนนต์ของ MIM It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases. คุณอาจสามารถแก้ไขปัญหาของคุณด้วยการซิงค์ MIM ถ้าปัญหาได้รับการแก้ไขในการอัปเดตล่าสุดเป็น MIM หรือเป็นหนึ่งในปัญหาอื่นๆ ที่กล่าวถึงในส่วนด้านล่าง

**ขั้นตอนที่แนะนา**

1. ตรวจสอบให้แน่ใจว่าคุณได้ใช้การอัปเดตล่าสุดของการซิงค์ MIM และตรวจสอบบันทึกย่อการเปิดตัวการซิงค์ [MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) เพื่อตรวจสอบว่าปัญหาได้รับการแก้ไขในการอัปเดตหรือไม่
2. ถ้าปัญหาอยู่กับทั่วไป LDAP, Generic SQL, Lotus Domino หรือตัวเชื่อมต่อบริการเว็บ ตรวจสอบให้แน่ใจว่าคุณใช้การอัปเดตล่าสุดของ [ตัวเชื่อมต่อ](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)ทั่วไป
3. ถ้าการซิงค์ MIM หยุดที่มีข้อผิดพลาด ให้ดูตารางรหัสข้อผิดพลาด [การเรียกใช้](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) เพื่อระบุสาเหตุที่อาจเกิดขึ้น
4. ถ้าการเรียกใช้หยุดโดยมีข้อยกเว้นส่วนขยาย **dll** ให้คลิกที่ข้อความเหล่านั้นเพื่อเปิดหน้าต่างคุณสมบัติวัตถุ Space **Connector** แล้วคลิกที่ **Stack Trace...** เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับสาเหตุพื้นฐาน ตามที่อธิบายไว้ในข้อยกเว้นส่วนขยาย [-DLL](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)
5. ถ้าคอมโพเนนต์ของบริการการแจ้งให้ทราบการเปลี่ยนแปลงรหัสผ่าน (PCNS) รายงานข้อผิดพลาด **6025** ในบันทึกเหตุการณ์ระหว่างการซิงโครไนซ์รหัสผ่าน ให้ตรวจสอบคู่มือการแก้ไขปัญหาข้อผิดพลาดการรายงาน [PCNS 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. ถ้าการซิงโครไนซ์กับตัวแทนการจัดการบริการ FIM ช้า ให้ตรวจสอบการตั้งค่าเพิ่มโดยอัตโนมัติของ TempDB ตามที่อธิบายไว้ใน การแก้ไขปัญหาช้าหรือหยุดการตอบสนอง[การซิงโครไนซ์](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)ทั้งหมด
7. ถ้าคุณพบข้อผิดพลาดของเซิร์ฟเวอร์ที่หยุดเมื่อเกิดข้อผิดพลาดในการสร้างผ่านบริการเว็บโดยใช้ตัวแทนการจัดการบริการ FIM ให้ดูข้อมูลสนับสนุน: การสร้างล้มเหลวผ่าน [บริการ](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) เว็บเพื่อดูภาพรวมของสาเหตุ

