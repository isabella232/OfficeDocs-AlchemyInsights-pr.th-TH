---
title: นโยบายกลุ่ม
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: 5bccaedda08e2c948a15c0b32c6f6eeecfc8bd4c4555b25291f294fe5deb3019
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088811"
---
# <a name="group-policy"></a>นโยบายกลุ่ม

การตั้งค่าวัตถุของผู้ใช้และคอมพิวเตอร์ใน Azure Active Directory Domain Services (Azure AD DS) มักจะได้รับการจัดการโดยใช้ Group Policy Objects (GPOs) Azure AD DS มี GPOs ในตัวของผู้ใช้ AADDC และคอนเทนเนอร์คอมพิวเตอร์ AADDC คุณสามารถกําหนดค่า GPOs ที่มีอยู่แล้วภายในเหล่านี้เพื่อกําหนดค่านโยบายกลุ่มตามที่ต้องการในสภาพแวดล้อมของคุณ สมาชิกของกลุ่มผู้ดูแลระบบ Azure AD DC จะมีสิทธิ์การจัดการดูแลนโยบายกลุ่มในโดเมน Azure AD DS และยังสามารถสร้างหน่วย GPOs และหน่วยขององค์กร (OUs) แบบที่ปรับแต่งเองได้ For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

ในสภาพแวดล้อมแบบไฮบริด นโยบายกลุ่มที่กําหนดค่าในสภาพแวดล้อม AD DS ภายในองค์กรจะไม่ถูกซิงโครไนซ์กับ Azure AD DS เมื่อต้องการกําหนดการตั้งค่าการกําหนดค่าให้กับผู้ใช้หรือคอมพิวเตอร์ใน Azure AD DS ให้แก้ไขหนึ่งใน GPOs เริ่มต้นหรือสร้าง GPO แบบกําหนดเอง

บทความนี้ [จัดการนโยบายกลุ่ม](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) แสดงวิธีการติดตั้งเครื่องมือการจัดการนโยบายกลุ่ม วิธีแก้ไข GPOs ที่มีอยู่แล้วภายใน และวิธีการสร้าง GPOs แบบปรับแต่งเอง



