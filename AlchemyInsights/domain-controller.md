---
title: ตัวควบคุมโดเมน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901316"
---
# <a name="domain-controller"></a>ตัวควบคุมโดเมน

**ไม่สามารถเปิดใช้งาน AAD DS หรือการปรับใช้ที่ล้มเหลว**

เมื่อต้องการแก้ไขปัญหาของบริการ Azure AD domain (AAD DS) ไม่ได้ถูกเปิดใช้งานหรือไม่สามารถปรับใช้ได้ให้ทำตามขั้นตอนต่อไปนี้:

1. ถ้าคุณกำลังใช้เครือข่ายเสมือนที่มีอยู่แล้วให้ตรวจสอบ NSG ของคุณสำหรับกฎที่บล็อกพอร์ตที่จำเป็นในการซิงโครไนซ์ใน AAD DS https://aka.ms/aadds-networking ในพอร์ทัล
2. ตรวจสอบเพื่อดูว่าข้อความแสดงข้อผิดพลาดของคุณได้รับคำตอบในคู่มือการแก้ไขปัญหานี้ที่พร้อมใช้งาน  https://aka.ms/aadds-troubleshoot-enable หรือไม่
3. ลองปรับใช้บริการ Domain AD Azure ในเครือข่ายเสมือนใหม่
4. ทำตามคู่มือเริ่มต้นใช้งานเกี่ยวกับวิธีการปรับใช้ AAD DS ซึ่งพร้อมใช้งานที่[บทช่วยสอนการสร้างบริการ DOMAIN AD Azure](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)
5. ถ้าคุณกำลังมีปัญหาเกี่ยวกับการปรับใช้บริการ Domain AD Azure ให้ดูที่การ [แก้ไขปัญหาของบริการ DOMAIN Ad azure](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) เพื่อแก้ไขข้อผิดพลาดทั่วไปเพื่อช่วยให้คุณทำสิ่งต่างๆได้อีกครั้ง 

**ไม่สามารถปิดใช้งาน AAD DS ได้**

AAD-DS ไม่สามารถหยุดชั่วคราวได้ ถ้าคุณต้องการหยุดการใช้โดเมนที่มีการจัดการของคุณจะต้องถูกลบออก

ถ้าคุณพบปัญหาในการแก้ไขข้อความแสดงข้อผิดพลาดทั่วไปและขั้นตอนการแก้ไขปัญหาที่เกี่ยวข้องเพื่อช่วยให้คุณทำสิ่งต่างๆให้เสร็จได้ให้ดูที่ [แก้ไขปัญหาบริการโดเมน](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)ของ active Directory ของ Azure
