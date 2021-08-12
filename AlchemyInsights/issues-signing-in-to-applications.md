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
ms.openlocfilehash: e1fd31366f24331e74b7e35887c3275549a7a394b128da560ba7a76437979553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925688"
---
# <a name="issues-signing-in-to-applications"></a>ปัญหาในการลงชื่อเข้าใช้แอปพลิเคชัน

เมื่อต้องการตรวจหาสาเหตุหรือวินิจฉัยปัญหาที่เกี่ยวข้องกับการลงชื่อเข้าใช้ของผู้ใช้ ให้ทําตามขั้นตอนต่อไปนี้:

1. เปิดใช้ [การวินิจฉัยการ](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)ลงชื่อเข้าใช้
2. ค้นหาเหตุการณ์ที่จะวิเคราะห์โดยการใส่รายละเอียดที่คุณมีเกี่ยวกับผู้ใช้ แอปพลิเคชัน เวลาลงชื่อเข้าใช้ การร้องขอ ID หรือ ID สหสัมพันธ์
3. ตรวจสอบผลลัพธ์การวินิจฉัยที่แสดงรายละเอียดของสิ่งที่เกิดขึ้นและการดําเนินการที่คุณสามารถดําเนินการเพื่อเปลี่ยนแปลงได้ ถ้ามีการเปลี่ยนแปลงใดๆ ที่มีการเปลี่ยนแปลง

ต่อไปนี้คือปัญหาทั่วไปที่คุณอาจพบเมื่อลงชื่อเข้าใช้แอปพลิเคชัน:

1. คุณหรือผู้ใช้ **ลงชื่อเข้าใช้ Azure AD เสร็จสมบูรณ์แล้ว** แต่จะเห็นพร้อมท์ที่ไม่คาดคิด - ดูบทความพร้อมท์การยินยอม [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)ที่ไม่คาดคิดเมื่อลงชื่อเข้าใช้แอปพลิเคชันและข้อผิดพลาดที่ไม่คาดคิดเมื่อแสดงความยินยอม [กับ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)แอปพลิเคชัน
2. คุณหรือผู้ใช้ **ลงชื่อเข้าใช้** แอปพลิเคชันโดยตรง แต่ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันจากลิงก์ลึกบนพอร์ทัลแบบปรับแต่งเองหรือแผงการเข้าถึง : ดู แก้ไขปัญหาการลงชื่อเข้าใช้แอปพลิเคชัน [จากแอปของฉัน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)ของ Azure AD
3. คุณหรือ **ผู้ใช้เสร็จสิ้น** การลงชื่อเข้าใช้ Azure AD แต่แอปพลิเคชันแสดงข้อความแสดงข้อผิดพลาดและไม่อนุญาตให้ผู้ใช้เสร็จสิ้นการลงชื่อเข้าใช้: ปัญหาคือแอปไม่ยอมรับการตอบกลับที่ Azure AD ออกให้ ให้ [ปฏิบัติตามขั้นตอน](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) เหล่านี้เพื่อแก้ไขปัญหา
4. คุณหรือผู้ใช้ **ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันที่ไม่ใช่แกลเลอรีที่** กําหนดค่าไว้สําหรับการลงชื่อเข้าระบบครั้งเดียวด้วยรหัสผ่าน : ให้ปฏิบัติตามแนวทาง [ในขั้นตอน](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) เหล่านี้เพื่อแก้ไขปัญหา
5. คุณหรือผู้ใช้ **ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันแกลเลอรี Azure AD ที่กําหนดค่า** ไว้เพื่อให้การลงชื่อเข้าระบบครั้งเดียวของรหัสผ่าน : [ให้ปฏิบัติตามขั้นตอน](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) เหล่านี้เพื่อแก้ไขปัญหา
6. คุณหรือ **ผู้ใช้ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชัน Microsoft : ให้** ปฏิบัติตาม [ขั้นตอน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) เหล่านี้เพื่อแก้ไขปัญหา
7. คุณหรือ **ผู้ใช้ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันที่ไม่ใช่แกลเลอรีที่กําหนดค่าไว้เพื่อ** ลงชื่อเข้าระบบครั้งเดียวแบบติดต่อกับภายนอก : ให้ [ปฏิบัติตามขั้นตอน](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) เหล่านี้เพื่อแก้ไขปัญหา
8. คุณหรือ **ผู้ใช้ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชัน Azure AD Gallery ที่กําหนดค่าไว้** เพื่อลงชื่อเข้าระบบครั้งเดียวแบบติดต่อกับภายนอก : [ให้ปฏิบัติตาม](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) ขั้นตอนเหล่านี้เพื่อแก้ไขปัญหา
9. คุณหรือผู้ใช้ **ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันที่พัฒนาขึ้นเองได้**: ให้ปฏิบัติตาม [ขั้นตอน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) เหล่านี้เพื่อแก้ไขปัญหา
10. คุณหรือ **ผู้ใช้ไม่สามารถลงชื่อเข้าใช้แอปพลิเคชันภายในองค์กรโดยใช้พร็อกซีแอปพลิเคชัน Azure AD**: ให้ [ปฏิบัติตามขั้นตอน](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) เหล่านี้เพื่อแก้ไขปัญหา

