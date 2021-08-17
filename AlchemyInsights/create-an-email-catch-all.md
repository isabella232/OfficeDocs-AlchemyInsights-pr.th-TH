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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080765"
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
