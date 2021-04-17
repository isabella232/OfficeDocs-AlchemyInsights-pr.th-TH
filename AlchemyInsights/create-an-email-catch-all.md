---
title: สร้างอีเมลที่ติดตามทั้งหมด
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816219"
---
# <a name="create-an-email-catch-all"></a>สร้างอีเมลที่ติดตามทั้งหมด

การใช้สิ่งที่จับได้ทั้งหมดนั้นถูกกีดกันอย่างรัดกุม คุณควรแจ้งการตีกลับกลับไปยังผู้ส่งเพื่อแจ้งให้ผู้ส่งทราบว่าไม่สามารถส่งข้อความได้ตามที่อยู่เพื่อให้พวกเขาสามารถจัดการได้ คุณยังสามารถจํากัดกล่องจดหมายที่มีการตรวจสอบให้ติดตามเฉพาะที่อยู่อีเมลที่ถูกต้องเดิมเท่านั้น 

กล่องจดหมายที่จับได้ทั้งหมดจะได้รับสแปมที่ใช่และอาจเต็มในที่สุดถ้าไม่ได้รับการตรวจสอบอย่างใกล้ชิด (มีการจํากัดการรับ) 

ถ้าคุณตัดสินใจที่จะดําเนินการต่อ ให้ปฏิบัติตามขั้นตอนเหล่านี้:

1. สร้างกลุ่มการแจกจ่ายแบบไดนามิก&รวมถึง "ชนิดผู้รับทั้งหมด"

2. สร้างกล่องจดหมายเฉพาะเพื่อติดตามอีเมล ตัวอย่างเช่น catchall@domain.com อีเมล

3. For the specific domain, set the DomainType to "InternalRelay". If you later remove the catch all, be sure to set the domain back to Authoritative.

4. สร้างกฎการส่งผ่านของจดหมายดังต่อไปนี้:

    - ถ้าผู้ส่งคือ "ภายนอกองค์กร"
    - เปลี่ยนเส้นทางข้อความไปยัง Catchall@domain.com
    - ยกเว้นถ้าผู้รับเป็นสมาชิกของกลุ่ม allusers@domain.com (กลุ่มการแจกจ่ายมีสมาชิกทั้งหมด)
    - ตรวจสอบให้แน่ใจว่ากล่องจดหมายใหม่ถูกเพิ่มลงในกลุ่มการแจกจ่ายแบบไดนามิก
