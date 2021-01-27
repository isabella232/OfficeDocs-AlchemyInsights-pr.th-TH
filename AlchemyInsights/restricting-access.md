---
title: การจำกัดการเข้าถึง
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7769"
ms.openlocfilehash: 8af9546f219474e2382cd2436470385bf3ad31e8
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015011"
---
# <a name="restricting-access"></a>การจำกัดการเข้าถึง

1. สำหรับข้อมูลเกี่ยวกับวิธีการจำกัดการเข้าถึงแอปพลิเคชันให้ดู[ที่วิธีการ: จำกัดแอป AZURE ad ของคุณให้เป็นชุดของผู้ใช้ในผู้เช่า AZURE AD](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users)
1. เรียนรู้วิธีการตรวจสอบและจัดการสิทธิ์ของแอปพลิเคชัน [ดำเนินการกับแอปพลิเคชัน overprivileged หรือแอปพลิเคชันที่น่าสงสัยใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-application-permissions#control-access-to-an-application) มีการดำเนินการที่แตกต่างกันที่คุณสามารถดำเนินการเพื่อรักษาความปลอดภัยแอปพลิเคชันของคุณตามสถานการณ์สมมติ การดำเนินการเหล่านี้จะนำไปใช้กับแอปพลิเคชันทั้งหมดที่ถูกเพิ่มลงในผู้เช่า Azure Active directory (Azure AD) ของคุณผ่านทางผู้ใช้หรือความยินยอมของผู้ดูแลระบบ
1. [จัดการงานที่มอบหมายของผู้ใช้สำหรับแอปใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal#configure-an-application-to-require-user-assignment) แสดงวิธีการกำหนดผู้ใช้และกลุ่มให้กับแอปพลิเคชันสำหรับองค์กรใน Azure active Directory (azure AD) จากภายในพอร์ทัล azure หรือโดยใช้ PowerShell เมื่อคุณกำหนดผู้ใช้ให้กับแอปพลิเคชันแอปพลิเคชันจะปรากฏในแอปของผู้ใช้ของฉันเพื่อให้เข้าถึงได้ง่าย ถ้าแอปพลิเคชัน exposes บทบาทคุณยังสามารถกำหนดบทบาทที่เฉพาะเจาะจงให้กับผู้ใช้ได้ด้วย
    - สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการกำหนดผู้ใช้และกลุ่มให้ดูที่การ[เข้าถึงแบบมีเงื่อนไข: ผู้ใช้และกลุ่ม](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-users-groups)
