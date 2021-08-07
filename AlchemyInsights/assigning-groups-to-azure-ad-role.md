---
title: การกําหนดกลุ่มให้กับบทบาท Azure AD
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
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036259"
---
# <a name="assigning-groups-to-azure-ad-role"></a>การกําหนดกลุ่มให้กับบทบาท Azure AD

เมื่อต้องการกําหนดกลุ่ม Azure AD ที่มีแหล่งข้อมูลผู้ให้บริการออกใน Azure AD ไปยังบทบาท Azure AD ให้ปฏิบัติตามขั้นตอนต่อไปนี้:

1. สร้างกลุ่มใหม่ - เมื่อต้องการสร้างกลุ่มใหม่:

    a. ลงชื่อเข้าใช้ศูนย์การจัดการ Azure AD ด้วย **ผู้ดูแลระบบบทบาทที่มีสิทธิ์พิเศษ** หรือ **สิทธิ์ระดับ** ผู้ดูแลระบบส่วนกลาง
    b. เลือก **Azure Active Directory >กลุ่ม> กลุ่มทั้งหมด > กลุ่ม** ใหม่
    c. สร้างกลุ่ม

2. กําหนดบทบาทให้กับกลุ่มระหว่างการสร้างกลุ่มหรือหลังจากสร้างกลุ่ม

    a. เมื่อต้องการกําหนดบทบาทให้กับกลุ่มณ เวลาของการสร้างกลุ่ม คุณสามารถกําหนดบทบาท **Azure AD** ให้กับกลุ่มและสร้างกลุ่มได้
    b. เมื่อต้องการกําหนดบทบาทให้กับกลุ่มหลังจากสร้างบทบาทแล้ว ให้นําทางไปยังแท็บ **บทบาท** ที่มอบหมาย ของกลุ่มที่สร้างขึ้นใหม่ และกําหนดบทบาทให้กับกลุ่มนั้น  

**จัดการการเป็นสมาชิกของกลุ่มที่มอบหมายให้กับบทบาท Azure AD**

เมื่อต้องการป้องกันระดับสิทธิ์ ตามค่าเริ่มต้น เฉพาะผู้ดูแลระบบบทบาทที่มีสิทธิ์และผู้ดูแลระบบส่วนกลางเท่านั้นที่สามารถปรับเปลี่ยนการเป็นสมาชิกของกลุ่มที่มอบหมายให้กับบทบาทได้ อย่างไรก็ตาม พวกเขาสามารถเลือกกําหนดเจ้าของให้กับกลุ่มดังกล่าวและมอบหมายงานนี้ให้ผู้รับมอบสิทธิ์

For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). For more details on troubleshooting roles assigned to cloud groups, [see Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





