---
title: S/MIME ใน Outlook บนเว็บ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511527"
---
# <a name="encrypt-email-messages-in-outlook"></a>เข้ารหัสข้อความอีเมลใน Outlook

การเข้ารหัสลับข้อความ Microsoft 365 สร้างขึ้นบน Microsoft Azure จัดการสิทธิ์ (Azure RMS), ซึ่งเป็นส่วนหนึ่งของการป้องกันข้อมูล Azure ถ้าการสมัครใช้งานของคุณมีการจัดการสิทธิ์ Azure หรือการป้องกันข้อมูล Azure**คุณไม่จําเป็นต้องดําเนินการใดๆ เพื่อเปิดใช้งานหรือเปิดใช้งาน**บริการการจัดการสิทธิ์ด้วยตนเอง

โดยยึดตามคําติชมของลูกค้า เราจะไม่เปิดใช้งานกฎการรับส่งจดหมายของ Exchange เพื่อเข้ารหัสอีเมลขาออกที่มีข้อมูลที่สําคัญบางชนิดในผู้เช่าของคุณตามค่าเริ่มต้นอีกต่อไป แต่เราจะให้คําแนะนําโดยละเอียดเกี่ยวกับวิธีที่คุณสามารถทําได้เอง สําหรับรายละเอียดเพิ่มเติมเกี่ยวกับวิธีสร้างกฎการขนส่งเพื่อเข้ารหัสลับข้อมูลสําคัญ ให้ดู[บทความนี้](https://aka.ms/OmeEtr)

- ถ้าใช้ Outlook บนเว็บ (เดิม**คือ OWA):** เมื่อเขียนข้อความอีเมล เพียงคลิก**ป้องกัน**ใน OWA นี้จะนําไปใช้ "ไม่ส่งต่อ" สิทธิ์ คลิก**เปลี่ยนสิทธิ์**แล้วเลือก**เข้ารหัสลับ**เพื่อเข้ารหัสเฉพาะข้อความเท่านั้น

- ถ้าใช้**ไคลเอ็นต์ Outlook**: เมื่อต้องการส่งข้อความที่เข้ารหัสลับจาก Outlook 2013 หรือ 2016 หรือ Outlook 2016 for Mac ให้เลือก**ตัวเลือก**  >  **สิทธิ์**จากนั้นเลือกตัวเลือกการป้องกันที่คุณต้องการ

- เมื่อต้องการ**เข้ารหัสลับอีเมลทั้งหมดที่**ส่งไปยังผู้รับหรือองค์กรคู่ค้าภายนอกโดยอัตโนมัติ คุณจําเป็นต้องสร้างกฎการส่งจดหมายในศูนย์ดูแล Exchange คําแนะนําโดยละเอียดมีให้ใน[บทความสนับสนุนนี้](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

