---
title: ๗๒๖การบล็อกการส่งต่ออีเมล
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219874"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>การบล็อกหรือการยกเลิกการบล็อกการส่งต่ออีเมล

เมื่อต้องการเปิดหรือปิดใช้งานการส่งต่ออีเมลสำหรับกล่องจดหมายที่เฉพาะเจาะจงให้ดูที่[กำหนดค่าการส่งต่ออีเมล](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

ในระดับผู้เช่าการควบคุมการส่งต่อภายนอกจะเสร็จสมบูรณ์โดยใช้นโยบายการป้องกันสแปมขาออก ถ้าถูกตั้งค่าเป็นปิดหรืออัตโนมัติอาจเป็นการบล็อกการส่งต่ออีเมลด้วยข้อผิดพลาด "๕๕๐ 5.7.520 Access ถูกปฏิเสธองค์กรของคุณไม่อนุญาตให้มีการส่งต่อภายนอก" ในภายหลังถ้าการส่งต่อถูกตั้งค่าให้ถูกบล็อกนั่นเป็นข้อผิดพลาดที่ผู้ใช้ของคุณจะเห็น

ถ้าการส่งต่อถูกบล็อกโปรดตรวจสอบให้แน่ใจว่าได้กำหนดค่านโยบายให้เปิดใช้งาน Autoforward ภายนอก คุณสามารถตรวจสอบนโยบายตัวกรองสแปมขาออกจากศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายหรือโดยการเรียกใช้คำสั่ง HostedOutboundSpamFilterPolicy | ชื่อ fl, AutoForwardingMode ถ้าคุณต้องการตั้งค่าการบล็อก Autoforward คำสั่งเดียวกันจะบอกสถานะของนโยบายในตอนนี้

หมายเหตุ: ขอแนะนำให้ปิดใช้งาน Autoforward ภายนอกในนโยบายตัวกรองสแปมขาออกเริ่มต้นของคุณและเปิดใช้งานสำหรับผู้ใช้ที่ต้องการการส่งต่อภายนอกโดยการสร้างนโยบายแบบกำหนดเองสำหรับผู้ใช้เหล่านั้น คุณสามารถอ่านเพิ่มเติมได้ในการ[กำหนดค่าการส่งต่ออีเมลภายนอกใน Office ๓๖๕](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)