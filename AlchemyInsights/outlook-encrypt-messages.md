---
title: S/MIME ใน Outlook บนเว็บ
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010743"
---
# <a name="encrypt-email-messages-in-outlook"></a>เข้ารหัสลับข้อความอีเมลในOutlook

Microsoft 365 การเข้ารหัสลับข้อความถูกสร้างขึ้นบน Microsoft Azure Rights Management (Azure RMS) ซึ่งเป็นส่วนหนึ่งของ Azure Information Protection ถ้าการสมัครใช้งานของคุณมี Azure Rights Management หรือ Azure Information Protection คุณไม่ต้ิต้องทําการ **ใดๆ เพื่อเปิดใช้งานหรือเปิดใช้งาน** บริการการจัดการสิทธิ์ด้วยตนเอง

ตามความคิดเห็นของลูกค้า เราจะไม่เปิดใช้งานกฎลExchangeอีเมลเพื่อเข้ารหัสลับอีเมลขาออกที่มีข้อมูลที่ละเอียดอ่อนบางชนิดในผู้เช่าของคุณโดยอัตโนมัติตามค่าเริ่มต้น แต่เราจะให้คําแนะนําโดยละเอียดเกี่ยวกับวิธีที่คุณสามารถเพื่อตัวคุณเอง For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).

- ถ้าคุณใช้Outlookบนเว็บ (ชื่อเดิมคือ **OWA):** เมื่อเขียนข้อความอีเมล เพียงแค่ **คลิก ป้องกัน** ใน OWA การนี่จะใช้สิทธิ์ "อย่าส่งต่อ" **คลิก เปลี่ยน** สิทธิ์ **แล้วเลือก** เข้ารหัสลับ เพื่อเข้ารหัสลับเฉพาะข้อความ

- หาก **ใช้Outlookไคลเอ็นต์** ของคุณ : เมื่อต้องการส่งข้อความที่เข้ารหัสลับจาก Outlook 2013 หรือ 2016 หรือ Outlook 2016 for Mac ให้เลือก สิทธิ์  >  ตัวเลือก แล้วเลือกตัวเลือกการป้องกันที่คุณต้องการ

- เมื่อต้องการ **เข้ารหัสลับอีเมลทั้งหมดที่ส่งไปยัง** ผู้รับหรือองค์กรคู่ค้าภายนอกบางองค์กรโดยอัตโนมัติ คุณ need to create a mail flow transport rule in the Exchange admin center มีคําแนะนํา [โดยละเอียดอยู่ในบทความสนับสนุน](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)นี้

