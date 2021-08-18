---
title: บล็อกหรือยกเลิกการบล็อกการส่งต่ออีเมลอัตโนมัติภายนอก
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
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897487"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>บล็อกหรือยกเลิกการบล็อกการส่งต่ออีเมลอัตโนมัติ

เมื่อต้องการเปิดใช้งานหรือปิดใช้งานการส่งต่ออีเมลของกล่องจดหมายที่ระบุ ให้ดู [กําหนดค่าการส่งต่อ](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)อีเมล

ผู้ดูแลระบบสามารถควบคุมการส่งต่อภายนอกขององค์กรได้โดยใช้ [นโยบายสแปม](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)ขาออก คุณจัดการนโยบายสแปมขาออกในพอร์ทัล Microsoft 365 Defender ที่หรือโดยใช้ <https://security.microsoft.com/antispam> cmdlet [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)ใน Exchange Online PowerShell

ถ้าคุณได้รับข้อผิดพลาดต่อไปนี้: **"550 5.7.520 Access** ถูกปฏิเสธ องค์กรของคุณไม่อนุญาตให้ส่งต่อภายนอก" ตรวจสอบให้แน่ใจว่า นโยบายถูกกําหนดค่าเพื่อเปิดใช้งานข้อความส่งต่ออัตโนมัติภายนอก

**หมายเหตุ**: เราขอแนะนนะค่าเริ่มต้น โดยอัตโนมัติ **-** ระบบควบคุมการตั้งค่ากฎการส่งต่อโดยอัตโนมัติในนโยบายตัวกรองสแปมขาออกเริ่มต้นของคุณ (การส่งต่อภายนอกอัตโนมัติจะถูกบล็อก การส่งต่ออัตโนมัติภายในยังคงใช้งานได้) คุณควรสร้างนโยบายตัวกรองสแปมขาออกแบบเอง และใช้ค่า **เปิด - การส่งต่อ จะ** เปิดใช้งานเฉพาะผู้ใช้ที่ต้องการการส่งต่ออีเมลอัตโนมัติภายนอก For more information, see [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
