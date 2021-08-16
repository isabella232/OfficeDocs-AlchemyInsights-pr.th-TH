---
title: ปัญหาการเข้าถึงตามเงื่อนไข
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069983"
---
# <a name="conditional-access-issues"></a>ปัญหาการเข้าถึงตามเงื่อนไข

**แก้ไขปัญหาเกี่ยวกับการวินิจฉัยการลงชื่อเข้าใช้**

คุณสามารถค้นหาสิ่งที่เกิดขึ้นหรือวินิจฉัยปัญหาที่เกี่ยวข้องกับการลงชื่อเข้าใช้ของผู้ใช้ได้อย่างรวดเร็วโดยใช้ [การวินิจฉัยการลงชื่อเข้าใช้](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. เปิดใช้การวินิจฉัยการลงชื่อเข้าใช้
1. ค้นหาเหตุการณ์ที่จะวิเคราะห์โดยการใส่รายละเอียดที่คุณมีเกี่ยวกับผู้ใช้ แอปพลิเคชัน เวลาของการลงชื่อเข้าใช้ รหัสการร้องขอ หรือ ID สหสัมพันธ์
1. ตรวจสอบผลลัพธ์การวินิจฉัยที่แสดงรายละเอียดของสิ่งที่เกิดขึ้นและการดําเนินการที่คุณสามารถดําเนินการเพื่อเปลี่ยนแปลงได้ (ถ้ามีการเปลี่ยนแปลงใดๆ ที่ต้องใช้)

**ขั้นตอนการแก้ไขปัญหาการลงชื่อเข้าใช้** 

1. นําทางไปยังหน้าลงชื่อเข้าใช้ Azure AD
1. กรองการลงชื่อเข้าใช้ตามผู้ใช้ ช่วงเวลา แอปพลิเคชัน สถานะ แอปไคลเอ็นต์ และอื่นๆ
1. เลือกเหตุการณ์การลงชื่อเข้าใช้และดูแท็บ การเข้าถึงตามเงื่อนไข เพื่อดูว่านโยบายใดถูกประเมิน
1. คลิกแถวของนโยบายเพื่อดูรายละเอียดนโยบายและเข้าใจว่าเหตุใดนโยบายจึงถูกใช้งาน

**เครื่องมือในการแก้ไขปัญหานโยบายการเข้าถึงตามเงื่อนไข**

- โหมดรายงานเท่านั้นจะช่วยให้คุณสามารถประเมินนโยบายโดยไม่ส่งผลกระทบต่อผู้ใช้
- เครื่องมือ #A0 ช่วยให้คุณสามารถจําลองเหตุการณ์การลงชื่อเข้าใช้และดูนโยบายที่ปรับใช้
- Insightsและเวิร์กบุ๊กการรายงานจะแสดงผลกระทบแบบเรียลไทม์ของแต่ละนโยบาย

**นโยบายการป้องกันข้อมูลพื้นฐาน**

นโยบายการป้องกันข้อมูลพื้นฐานไม่ได้สนับสนุน โดยรายการเหล่านี้จะไม่ถูกบังคับใช้อีกต่อไปและจะถูกเอาออกจากพอร์ทัล Azure เร็วๆ นี้ เราขอแนะ[นนะให้เปิดใช้งานค่าเริ่มต้นด้านความปลอดภัย](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

ดูข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงตามเงื่อนไขที่:

[หลักปฏิบัติที่ดีที่สุดเพื่อการเข้าถึงตามเงื่อนไขในAzure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [เงื่อนไขในการเข้าถึงตามเงื่อนไข](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [ตัวควบคุมในการเข้าถึงตามเงื่อนไข](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [ที่ตั้งในการเข้าถึงตามเงื่อนไข](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
