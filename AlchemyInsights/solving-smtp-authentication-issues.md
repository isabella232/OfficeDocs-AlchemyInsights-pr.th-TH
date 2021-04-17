---
title: แก้ไขปัญหาการรับรองความถูกต้องของ SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826434"
---
# <a name="solving-smtp-authentication-issues"></a>แก้ไขปัญหาการรับรองความถูกต้องของ SMTP

ถ้าคุณได้รับข้อผิดพลาด 5.7.57 หรือ 5.7.3 เมื่อพยายามส่งอีเมล SMTP และรับรองความถูกต้องด้วยไคลเอ็นต์หรือแอปพลิเคชัน มีบางสิ่งที่คุณควรตรวจสอบ:

- การส่ง SMTP ที่ได้รับการรับรองความถูกต้องอาจถูกปิดใช้งานในผู้เช่าของคุณ หรือบนกล่องจดหมายที่คุณพยายามใช้ (ตรวจสอบทั้งสองการตั้งค่า) เมื่อต้องการอ่านเพิ่มเติม ให้ดู เปิดใช้งาน [หรือปิดใช้งานการส่ง SMTP ของไคลเอ็นต์ที่ได้รับการรับรอง](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)ความถูกต้อง

- ตรวจสอบว่าเปิดใช้งาน [ค่าเริ่มต้นความปลอดภัยของ Azure ให้](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) ผู้เช่าของคุณหรือไม่ ถ้าเปิดใช้งาน การรับรองความถูกต้อง SMTP โดยใช้การรับรองความถูกต้องพื้นฐาน (หรือที่เรียกว่าแบบดั้งเดิม ซึ่งจะใช้ชื่อผู้ใช้และรหัสผ่าน) จะล้มเหลว
