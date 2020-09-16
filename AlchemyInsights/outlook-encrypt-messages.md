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
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772317"
---
# <a name="encrypt-email-messages-in-outlook"></a>การเข้ารหัสลับข้อความอีเมลใน Outlook

การเข้ารหัสลับข้อความ microsoft ๓๖๕ถูกสร้างขึ้นบน Microsoft Azure Rights Management (Azure RMS) ซึ่งเป็นส่วนหนึ่งของการป้องกันข้อมูล Azure ถ้าการสมัครใช้งานของคุณมีการจัดการสิทธิ์ Azure หรือการป้องกันข้อมูล Azure **คุณไม่จำเป็นต้องดำเนินการใดๆในการเปิดใช้งานหรือเปิด** ใช้งานบริการการจัดการสิทธิ์ด้วยตนเอง

โดยยึดตามคำติชมของลูกค้าเราจะไม่เปิดใช้งานกฎการไหลของ Exchange mail อีกต่อไปเพื่อเข้ารหัสลับอีเมลขาออกโดยอัตโนมัติที่มีข้อมูลที่สำคัญบางชนิดในผู้เช่าของคุณตามค่าเริ่มต้น เราจะให้คำแนะนำโดยละเอียดเกี่ยวกับวิธีที่คุณสามารถทำได้ สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับวิธีการสร้างกฎการขนส่งเพื่อเข้ารหัสลับข้อมูลที่สำคัญให้ดู[บทความนี้](https://aka.ms/OmeEtr)

- ถ้าใช้ Outlook บนเว็บ (ชื่อเดิมคือ **OWA**): เมื่อเขียนข้อความอีเมลเพียงแค่คลิก **ป้องกัน** ใน OWA การดำเนินการนี้จะใช้สิทธิ์ "ไม่ส่งต่อ" คลิก **เปลี่ยนแปลงสิทธิ์** แล้วเลือก **เข้ารหัสลับ** เฉพาะข้อความที่เข้ารหัสลับ

- ถ้าใช้**ไคลเอ็นต์ Outlook**: เมื่อต้องการส่งข้อความที่เข้ารหัสลับจาก outlook ๒๐๑๓หรือ๒๐๑๖หรือ Outlook ๒๐๑๖ for Mac ให้เลือกสิทธิ์**ตัวเลือก**  >  **Permissions**จากนั้นเลือกตัวเลือกการป้องกันที่คุณต้องการ

- เมื่อต้องการ **เข้ารหัสลับอีเมลทั้งหมด** ที่ส่งไปยังผู้รับบางรายหรือองค์กรคู่ค้าภายนอกโดยอัตโนมัติคุณจำเป็นต้องสร้างกฎการขนส่งจดหมายเวียนในศูนย์การจัดการ Exchange คำแนะนำโดยละเอียดจะมีให้ใน[บทความสนับสนุนนี้](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)

