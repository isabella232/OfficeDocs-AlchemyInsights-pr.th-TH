---
title: ปัญหาเกี่ยวกับการเข้าถึงตามเงื่อนไข
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
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015004"
---
# <a name="conditional-access-issues"></a>ปัญหาเกี่ยวกับการเข้าถึงตามเงื่อนไข

**แก้ไขปัญหาเกี่ยวกับการวินิจฉัยการเข้าสู่ระบบ**

คุณสามารถค้นหาสิ่งที่เกิดขึ้นหรือวินิจฉัยปัญหาที่เกี่ยวข้องกับการลงชื่อเข้าใช้ของผู้ใช้โดยใช้การ [วินิจฉัยการเข้าสู่ระบบ](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)ได้อย่างรวดเร็ว:

1. เปิดใช้งานการวินิจฉัยการลงชื่อเข้าใช้
1. ค้นหาเหตุการณ์ในการวิเคราะห์โดยการใส่รายละเอียดที่คุณมีเกี่ยวกับผู้ใช้แอปพลิเคชันเวลาของการลงชื่อเข้าใช้ Id คำขอหรือ Id สหสัมพันธ์
1. ตรวจทานผลลัพธ์การวินิจฉัยแสดงรายละเอียดของสิ่งที่เกิดขึ้นและการดำเนินการที่คุณสามารถทำได้เพื่อทำการเปลี่ยนแปลง (ถ้าจำเป็นต้องมีการเปลี่ยนแปลง)

**ขั้นตอนในการแก้ไขปัญหาการลงชื่อเข้าใช้** 

1. นำทางไปยังหน้าการลงชื่อเข้าใช้ Azure AD
1. ตัวกรองการลงชื่อเข้าใช้โดยผู้ใช้ช่วงเวลาแอปพลิเคชันสถานะแอปพลิเคชันไคลเอ็นต์และอื่นๆ
1. เลือกเหตุการณ์การลงชื่อเข้าใช้และดูแท็บการเข้าถึงแบบมีเงื่อนไขเพื่อดูว่านโยบายใดที่ได้รับการประเมิน
1. คลิกแถวของนโยบายเพื่อดูรายละเอียดนโยบายและทำความเข้าใจว่าทำไมจึงนำไปใช้

**เครื่องมือในการแก้ไขปัญหานโยบายการเข้าถึงแบบมีเงื่อนไข**

- โหมดรายงานเท่านั้นให้คุณประเมินนโยบายโดยไม่มีผลกระทบต่อผู้ใช้
- เครื่องมืออะไรที่ช่วยให้คุณสามารถจำลองเหตุการณ์การลงชื่อเข้าใช้และดูว่ามีการนำนโยบายไปใช้
- เวิร์กบุ๊กข้อมูลเชิงลึกและการรายงานจะแสดงผลกระทบแบบเรียลไทม์ของนโยบายแต่ละรายการ

**นโยบายการป้องกันพื้นฐาน**

นโยบายการป้องกันพื้นฐานได้รับการสนับสนุน พวกเขาจะไม่ถูกบังคับใช้อีกต่อไปและจะถูกเอาออกจากพอร์ทัล Azure ในเร็วๆนี้ เราขอแนะนำให้เปิดใช้งาน[ค่าเริ่มต้นด้านความปลอดภัย](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงแบบมีเงื่อนไขให้ดู:

[หลักปฏิบัติที่ดีที่สุดสำหรับการเข้าถึงแบบมีเงื่อนไขใน Azure Active directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [เงื่อนไขในการเข้าถึง](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 ตามเงื่อนไข [ตัวควบคุมในการเข้าถึง](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 แบบมีเงื่อนไข [ตำแหน่งที่ตั้งในการเข้าถึง](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)แบบมีเงื่อนไข
