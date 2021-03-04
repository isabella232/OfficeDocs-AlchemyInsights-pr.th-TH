---
title: แก้ไขปัญหา SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430212"
---
# <a name="troubleshoot-sspr"></a>แก้ไขปัญหา SSPR

**ฉันมีปัญหาในการกําหนดค่าการรีเซ็ตรหัสผ่าน**

- ถ้าคุณเป็นผู้ดูแลระบบและค้นหาวิธีการเปิดใช้งานการตั้งค่ารหัสผ่านใหม่แบบบริการตนเอง ให้ดู [บทช่วยสอนเปิดใช้งาน SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)เพื่อกําหนดค่าการตั้งค่ารหัสผ่านใหม่ให้กับองค์กรของคุณ คุณยังอาจต้องการตรวจสอบข้อ [ควรทราบด้าน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)สิทธิ์การใช้งาน คุณต้องได้รับมอบหมายสิทธิ์การใช้งานอย่างน้อยหนึ่งสิทธิ์ในองค์กรของคุณ
    - **ระบบคลาวด์เฉพาะผู้ใช้** - Office 365 (O365) ชําระเงิน SKU หรือ Azure AD Basic
    - **ผู้ใช้ระบบคลาวด์และ/หรือผู้ใช้ในองค์กร** - Azure AD Premium P1 หรือ P2, Enterprise Mobility + Security (EMS) หรือ Secure Productive Enterprise (SPE)
- หากมีข้อสงสัยเพิ่มเติมเกี่ยวกับการรีเซ็ตรหัสผ่านด้วยตนเอง โปรดดู FAQ[ของเรา](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**ฉันได้รับข้อความแสดงข้อผิดพลาด**

ตรวจทานบทความนี้เพื่อค้นหาข้อผิดพลาดทั่วไปและโซลูชัน: แก้ไขปัญหา [การตั้งค่ารหัสผ่านใหม่แบบบริการตนเอง](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**ฉันมีปัญหากับนโยบายการตั้งค่ารหัสผ่านใหม่ของฉัน**

- ถ้านโยบายรีเซ็ตรหัสผ่านของคุณไม่เป็นไปตามที่คาดไว้ หรือถ้าคุณมีข้อถามเกี่ยวกับนโยบายรีเซ็ตรหัสผ่าน ให้อ่านบทความนี้: นโยบายและข้อจํากัดของรหัสผ่าน[ใน Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)
- นโยบายการตั้งค่ารหัสผ่านใหม่จะไม่ใช้กับผู้ดูแลระบบ Microsoft บังคับใช้นโยบายรีเซ็ตรหัสผ่านสองทางเริ่มต้นอย่างรัดกุมให้กับบทบาทผู้ดูแลระบบ Azure ตรวจสอบให้แน่ใจว่าคุณได้ทดสอบกับผู้ใช้ที่ไม่ใช่ผู้ดูแลระบบ For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**ฉันไม่ต้องการให้ผู้ใช้ลงทะเบียนข้อมูลความปลอดภัยเพิ่มเติมเพื่อตั้งค่ารหัสผ่านใหม่**

คุณสามารถใส่ข้อมูลล่วงหน้า (แอตทริบิวต์อีเมลและโทรศัพท์) ให้กับผู้ใช้ของคุณโดยใช้ API, PowerShell หรือ Azure AD Connect เมื่อต้องการเรียนรู้วิธีอ่าน:

- [การปรับใช้การรีเซ็ตรหัสผ่านโดยไม่ให้ผู้ใช้ลงทะเบียน](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [การรีเซ็ตรหัสผ่านจะใช้ข้อมูลใด](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**ฉันต้องการให้ผู้ใช้ของฉันลงทะเบียนข้อมูลความปลอดภัยเพิ่มเติมของพวกเขาในการตั้งค่ารหัสผ่านใหม่**

1. ให้ผู้ใช้ของคุณลงทะเบียนข้อมูลความปลอดภัยของพวกเขาเพื่อรีเซ็ตรหัสผ่านด้วยตนเองโดยให้[ส่งaka.ms/ssprsetupให้พวกเขา](https://mysignins.microsoft.com/security-info)
1. หลังจากใส่ข้อมูลให้กับผู้ใช้ (โดยผู้ใช้หรือผู้ดูแลระบบ) ให้มอบสิทธิ์ผู้ใช้ของคุณในการaka.ms/ssprเพื่อให้ผู้ใช้สามารถตั้งค่ารหัสผ่าน[](https://passwordreset.microsoftonline.com/)ของพวกเขาใหม่ได้
1. If users are still experiencing problems they are mostly **federrated** or **password hash synch** users. ซึ่งหมายความว่าอาจมีปัญหากับบริการ Password Writeback