---
title: การกําหนดMIMบริการการซิงค์
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
ms.openlocfilehash: f834bead0b6f22dcadc808d45dcefe7f6571ef62c74b7fd97355157ca49542af
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978504"
---
# <a name="configure-mim-sync-service"></a>การกําหนดMIMบริการการซิงค์

Microsoft Identity Managerการซิงโครไนซ์MIM (MIM) เป็นคอมโพเนนต์ของMIM It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases. คุณอาจสามารถแก้ไขปัญหาของคุณเกี่ยวกับ MIM ซิงค์ ถ้าปัญหาได้รับการแก้ไขในการอัปเดตล่าสุดของ MIM หรือเป็นหนึ่งในปัญหาอื่นๆ ที่กล่าวถึงในส่วนด้านล่าง

**ขั้นตอนที่แนะนา**

1. ตรวจสอบให้แน่ใจว่าคุณใช้การอัปเดตล่าสุดของ MIM ซิงค์ และตรวจสอบบันทึกย่อMIMรุ่นซิงค์[](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history)เพื่อตรวจสอบว่าปัญหาได้รับการแก้ไขในการอัปเดตหรือไม่
2. ถ้าปัญหาอยู่กับตัวเชื่อมต่อ LDAP ทั่วไป, generic SQL, Lotus Domino หรือ Web Services ตรวจสอบให้แน่ใจว่าคุณใช้การอัปเดตล่าสุดของ[ตัวเชื่อมต่อ](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)ทั่วไป
3. ถ้ามีMIM หยุดการซิงคโดยมีข้อผิดพลาด ให้ดูตารางรหัสข้อผิดพลาด[การเรียกใช้](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes)เพื่อระบุสาเหตุที่อาจเกิดขึ้น
4. ถ้าการเรียกใช้หยุดโดยมีข้อยกเว้นส่วนขยาย **-dll** แล้วคลิกที่ข้อความเหล่านั้นเพื่อเปิดหน้าต่างคุณสมบัติ วัตถุช่องว่างตัวเชื่อมต่อ แล้วคลิกที่ **Stack Trace...** เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับสาเหตุพื้นฐาน ตามที่อธิบายไว้ใน [ข้อยกเว้นของส่วนขยาย DLL](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)
5. ถ้าคอมโพเนนต์ Password Change Notification Service (PCNS) รายงานข้อผิดพลาด **6025** ในบันทึกเหตุการณ์ระหว่างการซิงโครไนซ์รหัสผ่าน ให้ตรวจสอบคู่มือการแก้ไขปัญหาข้อผิดพลาดการรายงาน [PCNS 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. ถ้าการซิงโครไนซ์กับตัวแทนการจัดการบริการ FIM ช้า ให้ตรวจสอบการตั้งค่าขยายอัตโนมัติของ TempDB ตามที่อธิบายไว้ใน การแก้ไขปัญหาการซิงโครไนซ์แบบช้า[หรือแบบลอย](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)
7. ถ้าคุณพบข้อผิดพลาดของเซิร์ฟเวอร์ที่หยุดใช้งานด้วย failed-creation-via-web-services โดยใช้ตัวแทนการจัดการบริการ FIM ให้ดู ฝ่ายสนับสนุน [-ข้อมูล: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) เพื่อดูภาพรวมของสาเหตุ

