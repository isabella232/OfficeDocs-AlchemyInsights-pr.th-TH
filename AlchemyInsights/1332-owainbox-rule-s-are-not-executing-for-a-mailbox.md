---
title: 1332 OWA - กฎของกล่องขาเข้าจะไม่ดำเนินการสำหรับกล่องจดหมาย
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915823"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>กฎของกล่องขาเข้าไม่ทำงานตามที่คาดไว้

ตรวจสอบการตั้งค่าต่อไปนี้:
  
- ข้อความสามารถถูกเปลี่ยนเส้นทาง ส่งต่อ หรือโดยอัตโนมัติขึ้นอยู่กับกฎของกล่องขาเข้าเพียงครั้งเดียวเรียบร้อยแล้ว กฎการเปลี่ยนทิศทาง (ผิดกฎของกล่องขาเข้าหรือกระแสกฎสำหรับจดหมาย หรือที่เรียกอีกอย่างหนึ่งว่ากฎการขนส่ง) สามารถเพิ่มได้สูงสุดสิบการผู้รับส่งต่อข้อความ สำหรับข้อมูลเพิ่มเติม ให้ดู[สมุดรายวัน ขน ส่ง และอินบ็อกซ์ขีดจำกัดกฎ](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)
    
- กฎของกล่องขาเข้าไม่ทำงานกับกล่องจดหมายอื่นบันทึกนั้น สำหรับข้อมูลเพิ่มเติมเกี่ยวกับกล่องจดหมายบันทึกสำรอง ดู[กล่องจดหมายบันทึกสำรอง](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)
    
เมื่อต้องการแก้ไขปัญหาเหล่านี้ ดู[KB 2829319](https://support.microsoft.com/kb/2829319)
  
ถ้าไม่สามารถใช้กับปัญหาก่อนหน้านี้ เรียกใช้การวินิจฉัยรายงานกฎกล่องขาเข้าก่อนที่คุณเลื่อนระดับปัญหาไปยังฝ่ายสนับสนุนของ Microsoft:
  
1. เปิดกล่องจดหมายใน Outlook บนเว็บ และคลิกการ**ตั้งค่า** \> **ตัวเลือก** \> **จัดระเบียบอี** \> **กฎของกล่องขาเข้า**
    
2. ที่ด้านล่างของหน้า คลิก**ถ้ากฎของคุณกำลังทำงานอยู่ให้คลิกที่นี่เพื่อสร้างรายงานการวินิจฉัย**
    

