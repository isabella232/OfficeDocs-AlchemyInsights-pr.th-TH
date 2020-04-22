---
title: ข้อผิดพลาดในการส่งอีเมลที่ถูกบล็อกโดย SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714277"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>ข้อผิดพลาดในการส่งอีเมล: โฮสต์ไคลเอ็นต์ถูกบล็อกโดยใช้ Spamhaus

ที่อยู่ IP ที่ส่งข้อความอยู่ในรายชื่อบล็อกที่[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)เป็นเจ้าของ เหตุผลในการถูกบล็อกโดย Spamhaus ได้แก่ บัญชีที่ถูกบุกรุก เครื่องที่ถูกบุกรุกที่ใช้ที่อยู่ IP สาธารณะร่วมกัน และนโยบายผู้ให้บริการอินเทอร์เน็ต (ISP) การแก้ไขที่เป็นไปได้คือ:
  
- สําหรับข้อความขาเข้าที่ถูกบล็อกซึ่งคุณควบคุมเซิร์ฟเวอร์อีเมลต้นทาง คุณจําเป็นต้องระบุสาเหตุและลบบล็อกจากเว็บไซต์ Spamhaus

- สําหรับข้อความขาเข้าที่ถูกบล็อกซึ่งที่อยู่ IP ของแหล่งที่มาเป็นของบุคคลอื่นเจ้าของที่อยู่ต้องลบบล็อกจากเว็บไซต์ ถ้าอยู่ IP บนนโยบายบล็อกรายการ (PBL), เจ้าของสามารถกําหนดที่อยู่ IP แบบคงที่อื่น หรือเอาที่อยู่จาก PBL

- สําหรับข้อความขาออกที่ถูกบล็อกจากโดเมนของคุณที่เชื่อมต่อกับ Microsoft คุณสามารถรับข้อผิดพลาดนี้หากข้อความถูกส่งผ่านบริการของบริษัทอื่น คุณสามารถใช้เครื่องมือค้นหา WHOIS เพื่อค้นหาเจ้าของที่อยู่ IP ที่ถูกบล็อก
