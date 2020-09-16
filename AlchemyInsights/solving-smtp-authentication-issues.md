---
title: การแก้ไขปัญหาการรับรองความถูกต้องของ SMTP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 3eaab2c601f78e20f2ee67bc21a9598cb45a24f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738008"
---
# <a name="solving-smtp-authentication-issues"></a>การแก้ไขปัญหาการรับรองความถูกต้องของ SMTP

ถ้าคุณได้รับข้อผิดพลาด5.7.57 หรือ5.7.3 เมื่อพยายามส่งอีเมล SMTP และการรับรองความถูกต้องด้วยไคลเอ็นต์หรือแอปพลิเคชันมีบางสิ่งที่คุณควรตรวจสอบ:

- การส่งการรับรองความถูกต้องของ SMTP อาจถูกปิดใช้งานในผู้เช่าของคุณหรือในกล่องจดหมายที่คุณกำลังพยายามใช้ (ตรวจสอบการตั้งค่าทั้งสองอย่าง) เมื่อต้องการอ่านเพิ่มเติมให้ดูที่ [เปิดใช้งานหรือปิดใช้งานการส่ง SMTP ไคลเอ็นต์การรับรองความถูก](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)ต้อง

- ตรวจสอบว่า [ค่าเริ่มต้นของความปลอดภัย Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ถูกเปิดใช้งานสำหรับผู้เช่าของคุณหรือไม่ ถ้าเปิดใช้งานการรับรองความถูกต้องของ SMTP โดยใช้การรับรองความถูกต้องเบื้องต้น (หรือที่เรียกว่าเก่าการทำเช่นนี้จะใช้ชื่อผู้ใช้และรหัสผ่าน) จะล้มเหลว
