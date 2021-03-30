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
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405683"
---
# <a name="authentication-app"></a>แอปการรับรองความถูกต้อง

ถ้าคุณเป็นผู้ดูแลระบบส่วนกลาง คุณสามารถค้นหาสิ่งที่เกิดขึ้นหรือวินิจฉัยปัญหาที่เกี่ยวข้องกับการลงชื่อเข้าใช้ของผู้ใช้ได้อย่างรวดเร็วโดยใช้ [การวินิจฉัยการ](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)ลงชื่อเข้าใช้

1. เริ่มการวินิจฉัยโดยคลิกปุ่ม "[เปิดใช้การวินิจฉัย](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" 
1. ค้นหาเหตุการณ์ที่จะวิเคราะห์โดยการใส่รายละเอียดที่คุณมีเกี่ยวกับผู้ใช้ แอปพลิเคชัน เวลาลงชื่อเข้าใช้ ID การร้องขอ หรือ ID สหสัมพันธ์
1. ตรวจทานผลลัพธ์การวินิจฉัยซึ่งแสดงรายละเอียดของสิ่งที่เกิดขึ้นและการดําเนินการที่คุณสามารถดําเนินการเพื่อเปลี่ยนแปลงได้ ถ้ามีการเปลี่ยนแปลงใดๆ ที่ต้องใช้

**ตรวจสอบสถานการณ์สมมติที่เกี่ยวข้อง:**

1. ถ้าผู้ใช้ไม่ได้รับการแจ้งเตือนแบบพุชในแอป Microsoft Authenticator ให้ตรวจสอบว่าไม่ได้แสดงอยู่ภายใต้ผู้ใช้ที่ถูกบล็อก MFA ตามที่อธิบายไว้ในการบล็อกและยกเลิกการ[บล็อกผู้ใช้](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. ถ้าผู้ใช้ไม่ถูกบล็อกด้วย MFA แต่ไม่ได้รับการแจ้งเตือนแบบพุช พวกเขาจะสามารถเปิดแอป Microsoft Authenticator ซึ่งจะดึงการร้องขอการอนุมัติที่ค้างอยู่
1. ในฐานะที่เป็นวิธีการลงชื่อเข้าใช้อื่น ผู้ใช้ยังสามารถคลิกลงชื่อเข้าใช้ด้วยวิธีอื่นและเลือกใช้รหัสการตรวจสอบจากแอปบนอุปกรณ์เคลื่อนที่ของฉัน
1. แอป Microsoft Authenticator คือวิธีที่พร้อมใช้งานเฉพาะผู้ใช้หลายคนเท่านั้น [เรียนรู้เพิ่มเติมเกี่ยวกับค่าเริ่มต้นด้านความปลอดภัย ตรวจสอบ Faq](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)[ของแอป Authenticator](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq)เพื่อดูข้อถามที่ถามบ่อยและวิธีการแก้ไข
 
**วิดีโอที่แนะนนะ**

[วิธีการตั้งค่าแอป Authenticator บนโทรศัพท์เครื่องใหม่ (2 นาที)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
