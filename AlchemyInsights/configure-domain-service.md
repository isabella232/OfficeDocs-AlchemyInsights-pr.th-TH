---
title: กำหนดค่าบริการโดเมน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885685"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>ไม่สามารถเปิดใช้งาน AAD DS หรือการปรับใช้ที่ล้มเหลว

เมื่อต้องการแก้ไขปัญหาของบริการ Azure AD domain (AAD DS) ไม่ได้ถูกเปิดใช้งานหรือไม่สามารถปรับใช้ได้ให้ทำตามขั้นตอนต่อไปนี้:

1. ถ้าคุณกำลังใช้เครือข่ายเสมือนที่มีอยู่แล้วให้ตรวจสอบ NSG ของคุณสำหรับกฎที่บล็อกพอร์ตที่จำเป็นในการซิงโครไนซ์ใน AAD DS https://aka.ms/aadds-networking ในพอร์ทัล
2. ตรวจสอบเพื่อดูว่าข้อความแสดงข้อผิดพลาดของคุณได้รับคำตอบในคู่มือการแก้ไขปัญหานี้ที่พร้อมใช้งาน  https://aka.ms/aadds-troubleshoot-enable หรือไม่
3. ลองปรับใช้บริการ Domain AD Azure ในเครือข่ายเสมือนใหม่
4. ทำตามคู่มือการเริ่มต้นใช้งานในการปรับใช้ AAD DS:[สร้างและกำหนดค่าบริการ Domain Domain](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)
5. ถ้าคุณกำลังมีปัญหาเกี่ยวกับการปรับใช้บริการ Domain AD Azure ให้ดูที่การ [แก้ไขปัญหาของบริการ DOMAIN Ad azure](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) เพื่อแก้ไขข้อผิดพลาดทั่วไปเพื่อช่วยให้คุณทำสิ่งต่างๆได้อีกครั้ง 

**ไม่สามารถปิดใช้งาน AAD DS ได้**

AAD-DS ไม่สามารถหยุดชั่วคราวได้ ถ้าคุณต้องการหยุดการใช้โดเมนที่มีการจัดการของคุณจะต้องถูกลบออก
เมื่อต้องการลบโดเมนที่มีการจัดการของคุณให้ดู[ลบบริการโดเมน AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)



