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
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256908"
---
# <a name="group-policy"></a>นโยบายกลุ่ม

การตั้งค่าวัตถุผู้ใช้และคอมพิวเตอร์ใน Azure Active Directory Domain Services (Azure AD DS) มักจะได้รับการจัดการโดยใช้ Group Policy Objects (GPOs) Azure AD DS ประกอบด้วย GPOs ในตัวของผู้ใช้ AADDC และคอนเทนเนอร์คอมพิวเตอร์ AADDC คุณสามารถกําหนดค่า GPOs ที่มีอยู่แล้วภายในเหล่านี้เพื่อกําหนดค่านโยบายกลุ่มตามที่ต้องการในสภาพแวดล้อมของคุณ สมาชิกของกลุ่มผู้ดูแลระบบ Azure AD DC มีสิทธิ์การดูแลนโยบายกลุ่มในโดเมน Azure AD DS และยังสามารถสร้างหน่วย GPOs และหน่วยองค์กรแบบปรับแต่งเอง (OUs) ดูข้อมูลเพิ่มเติมเกี่ยวกับนโยบายกลุ่มและวิธีใช้งาน ดู [ภาพรวมของ](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))นโยบายกลุ่ม

ในสภาพแวดล้อมแบบไฮบริด นโยบายกลุ่มที่กําหนดค่าในสภาพแวดล้อม AD DS ภายในองค์กรจะไม่ถูกซิงโครไนซ์กับ Azure AD DS เมื่อต้องการกําหนดการตั้งค่าการกําหนดค่าให้กับผู้ใช้หรือคอมพิวเตอร์ใน Azure AD DS ให้แก้ไขหนึ่งใน GPOs เริ่มต้นหรือสร้าง GPO แบบกําหนดเอง

บทความนี้ [จัดการนโยบายกลุ่ม](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) แสดงวิธีการติดตั้งเครื่องมือการจัดการนโยบายกลุ่ม วิธีที่ ton แก้ไข GPOs ในตัว และวิธีการสร้าง GPOs แบบปรับแต่งเอง



