---
title: ปัญหาเกี่ยวกับข้อมูลรับรอง
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: 975d4850c1ecffae786dd19b7f4363e0c95378cff4f3ae6bb1968af33ef810b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986838"
---
# <a name="issues-with-credentials"></a>ปัญหาเกี่ยวกับข้อมูลรับรอง

แพลตฟอร์มข้อมูลประจําตัวของ Microsoftโฟลว์ข้อมูลรับรองความถูกต้องของไคลเอ็นต์[OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)จะอธิบายวิธีการเขียนโปรแกรมโดยตรงกับโฟลว์การให้ข้อมูลรับรองความถูกต้องของไคลเอ็นต์ OAuth 2.0

**ฉันจะจัดการรหัสผ่านหรือข้อมูลรับรองใบรับรองของแอปพลิเคชันได้อย่างไร**

ใน Azure CLI คุณสามารถใช้ข้อมูลรับรอง [ความถูกต้องของแอป az ad](https://docs.microsoft.com/cli/azure/ad/app/credential) เพื่อลบ รายการ หรือรีเซ็ตรหัสผ่านหรือข้อมูลรับรองใบรับรองของแอปพลิเคชันได้

**ผู้ใช้ของฉันจะตั้งค่ารหัสผ่านของพวกเขาใหม่ได้อย่างไร**

ผู้ใช้ต้อง [ลงทะเบียนตั้งค่ารหัสผ่านใหม่ด้วยตนเอง](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) ก่อน จึงจะสามารถตั้งค่ารหัสผ่านของพวกเขาใหม่ได้ เมื่อลงทะเบียนผู้ใช้แล้ว พวกเขาสามารถปฏิบัติตามคําแนะนําในบทความนี้เพื่อรีเซ็ตรหัสผ่าน: [รีเซ็ตรหัสผ่านที่โรงเรียนหรือที่โรงเรียน](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)ของคุณ

**ผู้ใช้ของฉันจะเปลี่ยนรหัสผ่านได้อย่างไร**

ผู้ใช้สามารถปฏิบัติตามขั้นตอนในบทความนี้เพื่อเปลี่ยนรหัสผ่านของพวกเขา: [วิธีเปลี่ยนรหัสผ่าน](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)ของคุณ
พวกเขายังสามารถ [จัดการรหัสผ่านแอปเพื่อการตรวจสอบสอง](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)ขั้นตอน

**ผู้ใช้ของฉันได้รับข้อผิดพลาดเมื่อเปลี่ยนแปลงหรือรีเซ็ตรหัสผ่านของพวกเขา**

ลิงก์นี้จะให้ข้อมูลเกี่ยวกับปัญหาทั่วไปที่อาจเกิดขึ้นเมื่อผู้ใช้พยายามตั้งค่ารหัสผ่านใหม่: [ปัญหาทั่วไปและโซลูชันของพวกเขา](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**ฉันพบปัญหาในการตั้งค่ารหัสผ่านของผู้ใช้ใหม่**

- ตรวจสอบให้แน่ใจว่าคุณได้รับอนุญาตให้ตั้งค่ารหัสผ่านใหม่ *เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านของผู้ใช้ใหม่ได้* ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์อื่นๆ ใหม่ได้

- ตรวจสอบให้แน่ใจว่าคุณเข้าใจความต้องการด้านสิทธิ์การใช้งานดังนี้

  - คุณต้องได้รับมอบหมายสิทธิ์การใช้งานอย่างน้อยหนึ่งสิทธิ์ในองค์กรของคุณ ดังนี้
    - **ระบบคลาวด์เฉพาะผู้ใช้**- บัญชีOffice 365 (O365) SKU ที่ชําระเงินแล้วหรือ Azure AD Basic
    - **ผู้ใช้ระบบคลาวด์และ/หรือผู้ใช้ภายในองค์กร**- Azure AD Premium P1 หรือ P2, Enterprise Mobility + Security (EMS) หรือ Secure Productive Enterprise (SPE)
    - To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).
- เมื่อต้องการรีเซ็ตรหัสผ่านของผู้ใช้ ให้ค้นหาผู้ใช้ใน Azure AD จากนั้น บนใบภาพรวมของผู้ใช้รายนั้น ให้คลิกปุ่ม "รีเซ็ตรหัสผ่าน"

**ปุ่มรีเซ็ตรหัสผ่านเป็นสีเทา**

คุณไม่ได้รับอนุญาตให้ **รีเซ็ต** รหัสผ่านของผู้ใช้นี้ *เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านของผู้ใช้ใหม่ได้* ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์อื่นๆ ใหม่ได้

**ฉันไม่เห็นเบลดรีเซ็ตรหัสผ่าน**

คุณไม่ได้รับอนุญาตให้ตั้งค่ารหัสผ่านใหม่ *เฉพาะผู้ดูแลระบบส่วนกลาง รหัสผ่าน และผู้ใช้เท่านั้นที่สามารถตั้งค่ารหัสผ่านของผู้ใช้ใหม่ได้* ผู้ดูแลระบบส่วนกลางยังสามารถตั้งค่ารหัสผ่านของผู้ดูแลระบบที่มีสิทธิ์อื่นๆ ใหม่ได้

**ฉันไม่เห็นเบลดการรวมภายในองค์กรในการรีเซ็ตรหัสผ่าน**

- เบลดการรวมภายในองค์กรจะปรากฏเฉพาะในสภาพแวดล้อมแบบไฮบริดเท่านั้น หมายความว่าคุณใช้การเขียนย้อนกลับของรหัสผ่านเพื่อจัดการรหัสผ่านของผู้ใช้ในองค์กร

- คุณไม่เห็นใบนี้หาก:

  - คุณไม่ได้ใช้ Writeback รหัสผ่าน
  - มีปัญหากับการติดตั้ง/การเชื่อมต่อการเขียนรหัสผ่านของคุณ
  - มีปัญหากับการติดตั้ง/การเชื่อมต่อของ Azure AD เชื่อมต่อ
  - For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**ฉันไม่รู้วิธีการตั้งค่ารหัสผ่านของผู้ใช้ใหม่**

1. ลงชื่อเข้าใช้พอร์ทัล Azure ในฐานะผู้ดูแลระบบที่เหมาะสม
2. ไปที่ **ตัวผู้ใช้และกลุ่ม** ให้เลือก **ผู้ใช้** ทั้งหมด
3. เลือกผู้ใช้จากรายการ
4. ผู้ใช้ที่เลือก ให้เลือก **ภาพรวม** จากนั้นในแถบสั่ง ให้เลือก **รีเซ็ต** รหัสผ่าน
5. เลือก **ปุ่ม รีเซ็ตรหัสผ่าน** แล้วปฏิบัติตามคําแนะนําบนหน้าจอ
    - เฉพาะการรีเซ็ตที่ผ่านพอร์ทัล **Azure เท่านั้น** ที่สนับสนุนการเขียนรหัสผ่าน

**ฉันตั้งค่ารหัสผ่านของผู้ใช้ภายในองค์กรใหม่จากพอร์ทัล Office 365 Admin หรือOffice 365อื่น แต่ผู้ใช้ยังคงไม่สามารถลงชื่อเข้าใช้ได้**

Password Writeback ไม่ได้รับการสนับสนุนในพอร์ทัลนี้ รีเซ็ตรหัสผ่านของผู้ใช้อีกครั้งในพอร์ทัล Azure
