---
title: การกําหนดค่าบริการโดเมน
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
ms.openlocfilehash: cf8ea7d73adf36f71ae92abad48ef9b664eb0c96094a38750c86cf42958b5323
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994788"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>ไม่สามารถเปิดใช้งาน AAD-DS หรือการปรับใช้ล้มเหลว

เมื่อต้องการแก้ไขปัญหาของบริการโดเมน Azure AD (AAD-DS) ที่ไม่ได้เปิดใช้งานหรือไม่สามารถปรับใช้ ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. ถ้าคุณใช้เครือข่ายเสมือนที่มีอยู่แล้ว ให้ตรวจสอบ NSG ของคุณดูกฎที่บล็อกพอร์ตที่ต้องใช้ในการซิงโครไนซ์ใน AAD-DS ใน https://aka.ms/aadds-networking พอร์ทัล
2. ตรวจสอบเพื่อดูว่าข้อความแสดงข้อผิดพลาดของคุณได้รับคําตอบในคู่มือการแก้ไขปัญหานี้ที่พร้อมใช้งานใน  https://aka.ms/aadds-troubleshoot-enable หรือไม่
3. ลองปรับใช้ Azure AD Domain Services ในเครือข่ายเสมือนใหม่
4. ปฏิบัติตามคู่มือการเริ่มต้นใช้งานเกี่ยวกับวิธีการปรับใช้ AAD-DS:[สร้างและกําหนดค่าบริการโดเมน AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)
5. ถ้าคุณพบปัญหาเกี่ยวกับการปรับใช้บริการโดเมน Azure AD ให้ดู [แก้ไขปัญหาบริการโดเมน Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) เพื่อแก้ไขข้อผิดพลาดทั่วไปเพื่อช่วยให้คุณแก้ไขปัญหาต่างๆ ที่ใช้งานได้อีกครั้ง 

**ไม่สามารถปิดใช้งาน AAD-DS ได้**

AAD-DS ไม่สามารถหยุดชั่วคราวได้ ถ้าคุณต้องการหยุดใช้โดเมนที่มีการจัดการของคุณ โดเมนนั้นต้องถูกลบ
เมื่อต้องการลบโดเมนที่มีการจัดการ ให้ดูที่[ลบบริการโดเมน AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)



