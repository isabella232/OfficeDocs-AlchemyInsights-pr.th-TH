---
title: แอปการรับรองความถูกต้อง
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082961"
---
# <a name="authentication-app"></a>แอปการรับรองความถูกต้อง

ถ้าคุณเป็นผู้ดูแลระบบส่วนกลาง คุณสามารถค้นหาสิ่งที่เกิดขึ้นหรือวินิจฉัยปัญหาที่เกี่ยวข้องกับการลงชื่อเข้าใช้ของผู้ใช้ได้อย่างรวดเร็วโดยใช้ [การวินิจฉัย](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)การลงชื่อเข้าใช้

1. เริ่มการวินิจฉัยโดยคลิกปุ่ม "[เปิดใช้การวินิจฉัย](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" 
1. ค้นหาเหตุการณ์ที่จะวิเคราะห์โดยการใส่รายละเอียดที่คุณมีเกี่ยวกับผู้ใช้ แอปพลิเคชัน เวลาของการลงชื่อเข้าใช้ รหัสการร้องขอ หรือ ID สหสัมพันธ์
1. ตรวจสอบผลลัพธ์การวินิจฉัยที่แสดงรายละเอียดของสิ่งที่เกิดขึ้นและการดําเนินการที่คุณสามารถดําเนินการเพื่อเปลี่ยนแปลงได้ ถ้ามีการเปลี่ยนแปลงใดๆ ที่มีการเปลี่ยนแปลง

**ตรวจสอบสถานการณ์สมมติที่เกี่ยวข้อง:**

1. ถ้าผู้ใช้ไม่ได้รับการแจ้งเตือนแบบพุชในแอป Microsoft Authenticator ให้ตรวจสอบว่าไม่ได้แสดงอยู่ภายใต้ผู้ใช้ที่ถูกบล็อก MFA ตามที่อธิบายไว้ใน บล็อกและยกเลิกการ[บล็อก](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)ผู้ใช้
1. ถ้าผู้ใช้ไม่ถูกบล็อกด้วย MFA แต่ไม่ได้รับการแจ้งเตือนแบบพุช ผู้ใช้จะสามารถเปิดแอป Microsoft Authenticator ซึ่งจะดึงการร้องขอการอนุมัติที่ค้างอยู่
1. ในฐานะที่เป็นวิธีการลงชื่อเข้าใช้อื่น ผู้ใช้ยังสามารถคลิก ลงชื่อเข้าใช้ด้วยวิธีอื่น และเลือกใช้รหัสการตรวจสอบจากแอปบนอุปกรณ์เคลื่อนที่ของฉัน
1. แอป Microsoft Authenticator แอปจะพร้อมใช้งานเฉพาะผู้ใช้หลายคนเท่านั้น [เรียนรู้เพิ่มเติมเกี่ยวกับค่าเริ่มต้นด้านความปลอดภัย ตรวจสอบAuthenticator](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)[ถามบ่อย](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq)เกี่ยวกับแอป เพื่อดูข้อถามที่ถามบ่อยและวิธีการแก้ไข
 
**วิดีโอที่แนะนา**

[วิธีการตั้งค่าแอปAuthenticatorบนโทรศัพท์เครื่องใหม่ (2 นาที)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
