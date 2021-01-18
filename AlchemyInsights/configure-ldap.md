---
title: กำหนดค่า LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885580"
---
# <a name="configure-ldap"></a>กำหนดค่า LDAP

เมื่อต้องการกำหนดค่า LDAP ให้ทำดังต่อไปนี้:

1. ตรวจสอบสถานภาพโดเมนของคุณบน[พอร์ทัล Azure](https://aka.ms/aadds-health)
1. ตรวจสอบให้แน่ใจว่าการสมัครใช้งาน Azure AD ที่ถูกต้องจะพร้อมใช้งานและบริการโดเมน AD Azure ได้ถูกเปิดใช้งาน
1. ใบรับรองที่จำเป็นต้องใช้ในการเปิดใช้งาน LDAP ที่ปลอดภัยต้องได้รับจากผู้ให้บริการออกใบรับรองสาธารณะที่เชื่อถือได้หรือเป็นใบรับรองแบบลงนามด้วยตนเอง
1. ตรวจสอบให้แน่ใจว่าใบรับรองเป็นไปตาม [แนวทาง](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)ที่จำเป็น

**ใบรับรองที่ไม่ถูกต้อง**
1. เมื่อต้องการต่ออายุใบรับรองให้ทำตามขั้นตอนในการสร้างใบรับรองและ reupload ใหม่:[กำหนดค่า LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. เมื่อต้องการแก้ไขปัญหาที่ทราบเกี่ยวกับการแจ้งเตือน LDAP ที่ปลอดภัยในบริการโดเมนของ active directory ของ Azure ให้ดูที่[แก้ไขการแจ้งเตือนของ ldap](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
