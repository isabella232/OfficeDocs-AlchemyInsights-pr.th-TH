---
title: ปัญหาในการลงชื่อเข้าใช้แอปพลิเคชัน
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901323"
---
# <a name="issues-signing-in-to-applications"></a>ปัญหาในการลงชื่อเข้าใช้แอปพลิเคชัน

เมื่อต้องการตรวจหาสาเหตุหรือวินิจฉัยปัญหาที่เกี่ยวข้องกับการลงชื่อเข้าใช้ของผู้ใช้ให้ทำตามขั้นตอนต่อไปนี้:

1. เปิดใช้งานการ[วินิจฉัยการลงชื่อเข้าใช้](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
2. ค้นหาเหตุการณ์ในการวิเคราะห์โดยการใส่รายละเอียดที่คุณมีเกี่ยวกับผู้ใช้แอปพลิเคชันเวลาของการลงชื่อเข้าใช้ Id คำขอหรือ Id สหสัมพันธ์
3. ตรวจทานผลลัพธ์การวินิจฉัยแสดงรายละเอียดของสิ่งที่เกิดขึ้นและการดำเนินการที่คุณสามารถทำได้เพื่อทำการเปลี่ยนแปลงถ้าจำเป็นต้องมีการเปลี่ยนแปลง

ต่อไปนี้คือปัญหาทั่วไปบางประการที่คุณอาจพบเมื่อลงชื่อเข้าใช้แอปพลิเคชัน:

1. คุณหรือผู้ใช้ **ได้ทำการลงชื่อเข้าใช้ AZURE AD เสร็จสมบูรณ์แล้วแต่จะเห็นการพร้อมท์ที่ไม่คาดคิดให้** ดูบทความ [พร้อมท์ความยินยอมที่ไม่คาดคิดเมื่อลงชื่อเข้าใช้แอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)และ [ข้อผิดพลาดที่ไม่คาดคิดเมื่อทำการยินยอมให้กับแอปพลิเคชัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
2. คุณหรือผู้ใช้ **ได้ลงชื่อเข้าใช้แอปพลิเคชันโดยตรงแต่ไม่สามารถลงชื่อเข้าใช้ได้จาก deeplink บนพอร์ทัลแบบกำหนดเองหรือแผงการเข้าถึง**: ดู [แก้ไขปัญหาการลงชื่อเข้าใช้แอปพลิเคชันจาก Azure AD Apps ของฉัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
3. คุณหรือผู้ใช้ทำ **การลงชื่อเข้าใช้ AZURE AD เสร็จสมบูรณ์แล้วแต่แอปพลิเคชันจะแสดงข้อความแสดงข้อผิดพลาดและไม่อนุญาตให้ผู้ใช้เสร็จสิ้นการเข้าสู่ระบบในการเข้าสู่ระบบ**: ปัญหานี้คือแอปไม่ยอมรับการตอบสนองที่ Azure AD ออก ทำตาม [ขั้นตอนต่อไปนี้](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) เพื่อแก้ไขปัญหา
4. คุณหรือผู้ใช้ **ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันที่ไม่ใช่แกลเลอรีที่ได้รับการกำหนดค่าสำหรับการลงชื่อเข้าใช้รหัสผ่านครั้งเดียว** ให้ทำตามคำแนะนำใน [ขั้นตอนเหล่านี้](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) เพื่อแก้ไขปัญหา
5. คุณหรือผู้ใช้ **ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันแกลเลอรี AD Azure ที่ได้รับการกำหนดค่าสำหรับการลงชื่อเข้าระบบครั้งเดียว** ให้ทำตาม [ขั้นตอนต่อไปนี้](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) เพื่อแก้ไขปัญหา
6. คุณหรือผู้ใช้ **ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชัน Microsoft**: ทำตาม [ขั้นตอนเหล่านี้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) เพื่อแก้ไขปัญหา
7. คุณหรือผู้ใช้ **ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันที่ไม่ใช่แกลเลอรีที่กำหนดค่าไว้สำหรับการลงชื่อเข้าใช้ครั้งเดียวที่ติดต่อกับภายนอก**: ทำตาม [ขั้นตอนเหล่านี้](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) เพื่อแก้ไขปัญหา
8. คุณหรือผู้ใช้ **ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันแกลเลอรี AD Azure ที่กำหนดค่าไว้สำหรับการลงชื่อเข้าใช้ครั้งเดียวที่ติดต่อกับภายนอก**: ทำตาม [ขั้นตอนเหล่านี้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) เพื่อแก้ไขปัญหา
9. คุณหรือผู้ใช้ **ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันที่ได้รับการพัฒนาแบบกำหนดเอง** ให้ทำตาม [ขั้นตอนเหล่านี้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) เพื่อแก้ไขปัญหา
10. คุณหรือผู้ใช้ **ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันภายในองค์กรโดยใช้พร็อกซีแอปพลิเคชัน AZURE AD**: ทำตาม [ขั้นตอนเหล่านี้](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) เพื่อแก้ไขปัญหา

