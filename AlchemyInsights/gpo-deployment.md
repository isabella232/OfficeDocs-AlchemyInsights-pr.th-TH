---
title: การปรับใช้ GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428050"
---
# <a name="gpo-deployment"></a>การปรับใช้ GPO

การตั้งค่าวัตถุผู้ใช้และคอมพิวเตอร์ใน Azure Active Directory Domain Services (Azure AD DS) มักจะได้รับการจัดการโดยใช้ Group Policy Objects (GPOs) Azure AD DS ประกอบด้วย GPOs ในตัวของผู้ใช้ AADDC และคอนเทนเนอร์คอมพิวเตอร์ AADDC คุณสามารถกําหนดค่า GPOs ที่มีอยู่แล้วภายในเหล่านี้เพื่อกําหนดค่านโยบายกลุ่มตามที่ต้องการในสภาพแวดล้อมของคุณ สมาชิกของกลุ่มผู้ดูแลระบบ Azure AD DC มีสิทธิ์การดูแลนโยบายกลุ่มในโดเมน Azure AD DS และยังสามารถสร้างหน่วย GPOs และหน่วยองค์กรแบบปรับแต่งเอง (OUs) ดูภาพรวมของนโยบายกลุ่มเพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับนโยบายกลุ่มและ [วิธี](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))ใช้งาน

ในสภาพแวดล้อมแบบไฮบริด นโยบายกลุ่มที่กําหนดค่าในสภาพแวดล้อม AD DS ภายในองค์กรจะไม่ถูกซิงโครไนซ์กับ Azure AD DS เมื่อต้องการกําหนดการตั้งค่าการกําหนดค่าให้กับผู้ใช้หรือคอมพิวเตอร์ใน Azure AD DS ให้แก้ไขหนึ่งใน GPOs เริ่มต้นหรือสร้าง GPO แบบกําหนดเอง

บทความนี้ [จัดการนโยบายกลุ่ม](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) แสดงวิธีการติดตั้งเครื่องมือการจัดการนโยบายกลุ่ม วิธีที่ ton แก้ไข GPOs ในตัว และวิธีการสร้าง GPOs แบบปรับแต่งเอง
