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
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053244"
---
# <a name="encrypt-email-messages-in-outlook"></a>เข้ารหัสข้อความทางเมลใน Outlook

การเข้ารหัสลับข้อความของ Office ๓๖๕ถูกสร้างขึ้นบน Microsoft Azure สิทธิ์การจัดการ (Azure RMS) ซึ่งเป็นส่วนหนึ่งของการป้องกันข้อมูล Azure ถ้าการสมัครสมาชิกของคุณมีการจัดการสิทธิ์ Azure หรือการป้องกันข้อมูล Azure**คุณไม่จำเป็นต้องดำเนินการใดๆเพื่อเปิดใช้งานหรือเปิดใช้**งานบริการการจัดการสิทธิ์ด้วยตนเอง

ขึ้นอยู่กับความคิดเห็นของลูกค้าเราจะไม่เปิดใช้งานกฎการไหลของจดหมาย Exchange เพื่อเข้ารหัสลับโดยอัตโนมัติที่มีบางชนิดของข้อมูลที่สำคัญในผู้เช่าของคุณโดยค่าเริ่มต้น แต่เราจะให้คำแนะนำโดยละเอียดเกี่ยวกับวิธีการที่คุณสามารถทำได้ด้วยตัวเอง สำหรับรายละเอียดเพิ่มเติมเกี่ยวกับวิธีการสร้างกฎการขนส่งเพื่อเข้ารหัสลับข้อมูลที่สำคัญโปรดดู[บทความนี้](https://aka.ms/OmeEtr)

- ถ้าใช้ Outlook บนเว็บ (เดิมคือ**OWA**): เมื่อเขียนข้อความทาง e-mail เพียงแค่คลิก**ป้องกัน**ใน OWA การดำเนินการนี้จะใช้ "อย่าส่งต่อ" ได้รับอนุญาต คลิ**กเปลี่ยนแปลงสิทธิ์**และเลือกเข้า**รหัส**เพื่อเข้ารหัสข้อความเท่านั้น

- ถ้าใช้**ไคลเอนต์ outlook**: เมื่อต้องการส่งข้อความที่เข้ารหัสลับจาก outlook ๒๐๑๓หรือ๒๐๑๖หรือ Outlook ๒๐๑๖สำหรับ Mac ให้เลือก**สิทธิ์****ตัวเลือก** > จากนั้นเลือกตัวเลือกการป้องกันที่คุณต้องการ

- หากต้องการเข้า**รหัสลับทั้งหมด**ที่ส่งไปยังผู้รับบางรายหรือองค์กรหุ้นส่วนภายนอกโดยอัตโนมัติ คำแนะนำโดยละเอียดจะมีให้ใน[บทความสนับสนุนนี้](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)

