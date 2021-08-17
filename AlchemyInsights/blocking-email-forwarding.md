---
title: 726 การบล็อกการส่งต่ออีเมล
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059651"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>การบล็อกหรือยกเลิกการบล็อกการส่งต่ออีเมล

เมื่อต้องการเปิดใช้งานหรือปิดใช้งานการส่งต่ออีเมลของกล่องจดหมายที่ระบุ ให้ดู [กําหนดค่าการส่งต่อ](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)อีเมล

ในระดับผู้เช่า การควบคุมการส่งต่อภายนอกจะเสร็จสิ้นโดยใช้นโยบายสแปมขาออก คุณสามารถตรวจสอบนโยบายตัวกรองสแปมขาออกจากศูนย์การรักษาความปลอดภัยและการปฏิบัติตามนโยบาย[ได้ที่นี่](https://protection.office.com/antispam)หรือโดยใช้สั่ง[Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

ถ้าคุณได้รับข้อผิดพลาดต่อไปนี้: "การเข้าถึง **550 5.7.520** ถูกปฏิเสธ องค์กรของคุณไม่อนุญาตให้ส่งต่อภายนอก" โปรดตรวจสอบให้แน่ใจว่าได้กําหนดค่านโยบายให้เปิดใช้งานการส่งต่อภายนอกโดยอัตโนมัติ

**หมายเหตุ:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users. คุณสามารถอ่านเพิ่มเติมใน การ[กําหนดค่าการส่งต่ออีเมลภายนอกOffice 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)