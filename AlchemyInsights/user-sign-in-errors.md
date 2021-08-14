---
title: ข้อผิดพลาดในการเข้าสู่ระบบของผู้ใช้
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
- "7790"
- "9004355"
ms.openlocfilehash: 09950bcbc96c95caff0d7b1b7c98373360a9900cd01fd6faf9e787f67cefb5a7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53990510"
---
# <a name="user-sign-in-errors"></a>ข้อผิดพลาดในการเข้าสู่ระบบของผู้ใช้

**แก้ไขปัญหาเกี่ยวกับการวินิจฉัยการลงชื่อเข้าใช้**

เมื่อต้องการตรวจหาสาเหตุหรือวินิจฉัยปัญหาที่เกี่ยวข้องกับการลงชื่อเข้าใช้ของผู้ใช้ ให้ทําตามขั้นตอนต่อไปนี้:

1. เปิดใช้ [การวินิจฉัยการ](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)ลงชื่อเข้าใช้
2. ค้นหาเหตุการณ์ที่จะวิเคราะห์โดยการใส่รายละเอียดที่คุณมีเกี่ยวกับผู้ใช้ แอปพลิเคชัน เวลาลงชื่อเข้าใช้ การร้องขอ ID หรือ ID สหสัมพันธ์
3. ตรวจสอบผลลัพธ์การวินิจฉัยที่แสดงรายละเอียดของสิ่งที่เกิดขึ้นและการดําเนินการที่คุณสามารถดําเนินการเพื่อเปลี่ยนแปลงได้ ถ้ามีการเปลี่ยนแปลงใดๆ ที่มีการเปลี่ยนแปลง

**ค้นหาข้อมูลเกี่ยวกับรหัสข้อผิดพลาด AADSTS ที่ส่งกลับจากบริการโทเค็นความปลอดภัยของ Azure Active Directory (Azure AD) (STS) อยู่ใช่หรือไม่** อ่านบทความ [นี้เพื่อค้นหา](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) รายละเอียดข้อผิดพลาด AADSTS การแก้ไข และวิธีแก้ไขปัญหาชั่วคราวที่แนะนะ