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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478325"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>การบล็อกหรือการยกเลิกการบล็อกการส่งต่ออีเมล

เมื่อต้องการเปิดหรือปิดใช้งานการส่งต่ออีเมลสำหรับกล่องจดหมายที่เฉพาะเจาะจงให้ดูที่[กำหนดค่าการส่งต่ออีเมล](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

ในระดับผู้เช่าการควบคุมการส่งต่อภายนอกจะเสร็จสมบูรณ์โดยใช้นโยบายสแปมขาออก คุณสามารถตรวจสอบนโยบายตัวกรองสแปมขาออกจากศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบายได้[ที่นี่](https://protection.office.com/antispam)หรือโดยใช้[คำสั่ง HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

ถ้าคุณได้รับข้อผิดพลาดต่อไปนี้: **"๕๕๐ 5.7.520 Access ถูกปฏิเสธองค์กรของคุณไม่อนุญาตให้มีการส่งต่อภายนอก"** โปรดตรวจสอบให้แน่ใจว่านโยบายถูกกำหนดค่าให้เปิดใช้งานการส่งต่อภายนอกโดยอัตโนมัติ

**หมายเหตุ:** ขอแนะนำให้ทำการปิดใช้งาน Autoforward ภายนอกในนโยบายตัวกรองสแปมขาออกเริ่มต้นของคุณและเปิดใช้งานเฉพาะสำหรับผู้ใช้ที่ต้องการการส่งต่อภายนอกโดยการสร้างนโยบายแบบกำหนดเองสำหรับผู้ใช้เหล่านั้น คุณสามารถอ่านเพิ่มเติมได้ในการ[กำหนดค่าการส่งต่ออีเมลภายนอกใน Office ๓๖๕](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)