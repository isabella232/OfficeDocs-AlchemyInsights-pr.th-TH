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
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038977"
---
# <a name="troubleshoot-sspr"></a>แก้ไขปัญหา SSPR

**ฉันมีปัญหาในการกําหนดค่าการรีเซ็ตรหัสผ่าน**

- ถ้าคุณเป็นผู้ดูแลระบบและค้นหาวิธีการเปิดใช้งานการรีเซ็ตรหัสผ่านแบบบริการตนเอง ให้ดู [บทช่วยสอนเปิดใช้งาน SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)เพื่อกําหนดค่าการตั้งค่ารหัสผ่านใหม่ให้กับองค์กรของคุณ นอกจากนี้ คุณอาจต้องการตรวจสอบข้อ[กฎหมายด้านสิทธิ์การใช้งาน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) คุณต้องมีสิทธิ์การใช้งานอย่างน้อยหนึ่งสิทธิ์ที่มอบหมายในองค์กรของคุณ
    - **ระบบคลาวด์เฉพาะผู้ใช้**- บัญชีOffice 365 (O365) SKU ที่ชําระเงินแล้วหรือ Azure AD Basic
    - **ผู้ใช้ระบบคลาวด์และ/หรือผู้ใช้ภายในองค์กร**- Azure AD Premium P1 หรือ P2, Enterprise Mobility + Security (EMS) หรือ Secure Productive Enterprise (SPE)
- หากมีข้อสงสัยเพิ่มเติมเกี่ยวกับการรีเซ็ตรหัสผ่านด้วยตนเอง โปรดดู FAQ[ของเรา](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)

**ฉันได้รับข้อความแสดงข้อผิดพลาด**

ดูบทความนี้เพื่อค้นหาข้อผิดพลาดทั่วไปและโซลูชัน: [แก้ไขปัญหาการรีเซ็ตรหัสผ่านด้วยตนเอง](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**ฉันมีปัญหากับนโยบายการตั้งค่ารหัสผ่านใหม่**

- ถ้านโยบายรีเซ็ตรหัสผ่านของคุณไม่เป็นไปตามที่คาดไว้ หรือถ้าคุณมีข้อถามเกี่ยวกับนโยบายการตั้งค่ารหัสผ่านใหม่ ให้อ่านบทความนี้: นโยบายและข้อจํากัดของรหัสผ่าน[ใน](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)Azure Active Directory
- นโยบายการตั้งค่ารหัสผ่านใหม่จะไม่ใช้กับผู้ดูแลระบบ Microsoft บังคับใช้นโยบายรีเซ็ตรหัสผ่านสองประตูเริ่มต้นอย่างรัดกุมของบทบาทผู้ดูแลระบบ Azure ตรวจสอบให้แน่ใจว่าคุณได้ทดสอบกับผู้ใช้ที่ไม่ใช่ผู้ดูแลระบบ For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**ฉันไม่ต้องการให้ผู้ใช้ของฉันลงทะเบียนข้อมูลความปลอดภัยเพิ่มเติมเพื่อรีเซ็ตรหัสผ่าน**

คุณสามารถใส่ข้อมูลล่วงหน้า (แอตทริบิวต์อีเมลและโทรศัพท์) ให้กับผู้ใช้ของคุณโดยใช้ API, PowerShell หรือ Azure AD เชื่อมต่อได้ เมื่อต้องการเรียนรู้วิธีการอ่าน:

- [การปรับใช้การรีเซ็ตรหัสผ่านโดยไม่ให้ผู้ใช้ลงทะเบียน](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [การรีเซ็ตรหัสผ่านจะใช้ข้อมูลใด](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**ฉันต้องการให้ผู้ใช้ลงทะเบียนข้อมูลความปลอดภัยเพิ่มเติมของตนเพื่อรีเซ็ตรหัสผ่าน**

1. ให้ผู้ใช้ของคุณลงทะเบียนข้อมูลความปลอดภัยของพวกเขาเพื่อรีเซ็ตรหัสผ่านด้วยตนเองโดยให้ขอให้พวกเขา[aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info)
1. หลังจากใส่ข้อมูลให้กับผู้ใช้ (โดยผู้ใช้หรือผู้ดูแลระบบ) ให้ให้ผู้ใช้ของคุณติดต่อ aka.ms/sspr เพื่อให้ผู้ใช้สามารถเพิ่มประสิทธิภาพในการ[](https://passwordreset.microsoftonline.com/)รีเซ็ตรหัสผ่านของพวกเขาเอง
1. If users are still experiencing problems they are mostly **fededrated or** **password hash synch** users. ซึ่งหมายความว่าอาจมีปัญหากับบริการ Password Writeback