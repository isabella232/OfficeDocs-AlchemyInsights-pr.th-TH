---
title: ปัญหาในการรีเซ็ตรหัสผ่าน
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: 535b5273d367e24ac45b3f60dbc7b6a2da6a3d9affa5a67499989d19a1904768
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039985"
---
# <a name="problems-resetting-password"></a>ปัญหาในการรีเซ็ตรหัสผ่าน

ต่อไปนี้คือปัญหาบางอย่างที่คุณอาจพบเมื่อรีเซ็ตรหัสผ่านและวิธีแก้ไขที่เป็นไปได้:

**ฉันมีปัญหากับการรีเซ็ตรหัสผ่านไม่ครอบคลุมในประเภทอื่นๆ**

- ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้รีเซ็ตรหัสผ่าน เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านของผู้ใช้ใหม่ได้ ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์อื่นๆ ใหม่ได้
- โปรดแน่ใจว่าคุณเข้าใจข้อกฎหมายด้านสิทธิ์การใช้งาน:
    - คุณต้องมีสิทธิ์การใช้งานอย่างน้อยหนึ่งสิทธิ์ที่มอบหมายในองค์กรของคุณ
        - ระบบคลาวด์เฉพาะผู้ใช้ - บัญชีOffice 365 (O365) SKU หรือ Azure AD Basic แบบชําระเงิน
        - ผู้ใช้ระบบคลาวด์และ/หรือผู้ใช้ภายในองค์กร - Azure AD Premium P1 หรือ P2, Enterprise Mobility + Security (EMS) หรือ Secure Productive Enterprise (SPE)
        - To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).

**ฉันพบปัญหาในการทดสอบนโยบายการตั้งค่ารหัสผ่านใหม่ที่ฉันตั้งค่าไว้**

- นโยบายที่ปรับใช้ล่าสุดอาจใช้เวลาหลายนาทีในข้อมูลในศูนย์ข้อมูลและจุดสิ้นสุดทั้งหมด ระยะทางจริงจากศูนย์ข้อมูลจะยังมีผลต่อวิธีการปรับใช้การเปลี่ยนแปลงอย่างรวดเร็วอีกด้วย
- ทดสอบกับผู้ใช้ปลายทาง ไม่ใช่ผู้ดูแลระบบ และทดสอบกับผู้ใช้กลุ่มเล็กๆ นโยบายที่กําหนดค่าในพอร์ทัล Azure จะมีผลบังคับใช้กับผู้ใช้เท่านั้น ไม่ใช่ผู้ดูแลระบบ Microsoft บังคับใช้นโยบายรีเซ็ตรหัสผ่านสองประตูเริ่มต้นอย่างรัดกุมให้กับบทบาทผู้ดูแลระบบ Azure (ตัวอย่าง: ผู้ดูแลระบบส่วนกลาง ผู้ดูแลระบบเจ้าหน้าที่ให้ความช่วยเหลือ ผู้ดูแลรหัสผ่าน เป็นต้น)
    - เรียนรู้เพ [ิ่มเติมเกี่ยวกับนโยบายของ](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)ผู้ดูแลระบบ

**ฉันต้องการปรับใช้การรีเซ็ตรหัสผ่าน แต่ฉันไม่ต้องการให้ผู้ใช้ของฉันลงทะเบียนข้อมูลความปลอดภัยเพิ่มเติม**

ใส่ข้อมูลล่วงหน้าให้กับผู้ใช้ของคุณ เพื่อให้พวกเขาไม่ต้อง! - ในฐานะผู้ดูแลระบบ คุณสามารถตั้งค่าคุณสมบัติโทรศัพท์และอีเมลให้กับผู้ใช้ของคุณก่อนที่จะเปิดตัวการตั้งค่ารหัสผ่านใหม่ให้กับองค์กรของคุณ คุณสามารถเรียกใช้ได้โดยใช้ API, PowerShell หรือ Azure AD เชื่อมต่อ ข้อมูลเพิ่มเติมที่นี่:
- [การปรับใช้การรีเซ็ตรหัสผ่านโดยไม่ให้ผู้ใช้ลงทะเบียน](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [การรีเซ็ตรหัสผ่านจะใช้ข้อมูลใด](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**ปุ่มรีเซ็ตรหัสผ่านเป็นสีเทา**

คุณไม่ได้รับอนุญาตให้รีเซ็ตรหัสผ่านของผู้ใช้นี้ เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านของผู้ใช้ใหม่ได้ ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์อื่นๆ ใหม่ได้

**ฉันไม่เห็นเบลดรีเซ็ตรหัสผ่าน**

คุณไม่ได้รับอนุญาตให้ตั้งค่ารหัสผ่านใหม่ เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านของผู้ใช้ใหม่ได้ ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์อื่นๆ ใหม่ได้

**ฉันไม่เห็นเบลดการรวมภายในองค์กรในการรีเซ็ตรหัสผ่าน**

- เบลดการรวมภายในองค์กรจะปรากฏเฉพาะในสภาพแวดล้อมแบบไฮบริดเท่านั้น หมายความว่าคุณใช้การเขียนย้อนกลับของรหัสผ่านเพื่อจัดการรหัสผ่านของผู้ใช้ในองค์กร
- คุณไม่เห็นใบนี้หาก:
    - คุณไม่ได้ใช้ Writeback รหัสผ่าน
    - มีปัญหากับการติดตั้ง/การเชื่อมต่อการเขียนรหัสผ่านของคุณ
    - มีปัญหากับการติดตั้ง/การเชื่อมต่อของ Azure AD เชื่อมต่อ
    - For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**ฉันไม่รู้วิธีการตั้งค่ารหัสผ่านของผู้ใช้ใหม่**

1. ลงชื่อเข้าใช้พอร์ทัล Azure ในฐานะผู้ดูแลระบบที่เหมาะสม
1. ไปที่ ตัวผู้ใช้และกลุ่ม ให้เลือก **ผู้ใช้** ทั้งหมด
1. เลือกผู้ใช้จากรายการ
1. ผู้ใช้ที่เลือก ให้เลือก **ภาพรวม** จากนั้นในแถบสั่ง ให้คลิก **ตั้งค่ารหัสผ่าน** ใหม่
1. ให้ปฏิบัติตามคําแนะนําบนหน้าจอ
    - เฉพาะการรีเซ็ตที่ผ่านพอร์ทัล Azure เท่านั้นที่สนับสนุนการเขียนรหัสผ่าน

**ฉันตั้งค่ารหัสผ่านของผู้ใช้ภายในองค์กรใหม่จากพอร์ทัล Office 365 Admin หรือOffice 365อื่น แต่ผู้ใช้ยังคงไม่สามารถลงชื่อเข้าใช้ได้**

Password Writeback ไม่ได้รับการสนับสนุนในพอร์ทัลนี้ รีเซ็ตรหัสผ่านของผู้ใช้อีกครั้งในพอร์ทัล Azure - portal.azure.com

