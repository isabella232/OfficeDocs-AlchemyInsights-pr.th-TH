---
title: Password Writeback ไม่ใช้งานได้
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
- "9004595"
- "8210"
ms.openlocfilehash: 679dea6d488cf74f51baee2b3b498dc64b95530e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324942"
---
# <a name="password-writeback-is-not-working"></a>Password Writeback ไม่ใช้งานได้

**ฉันมีปัญหาในการกําหนดค่า Writeback ของรหัสผ่าน**

- Password writeback คือฟีเจอร์ระดับพรีเมียม
- ตรวจสอบให้แน่ใจว่าคุณเข้าใจความต้องการด้านสิทธิ์การใช้งานดังนี้
  - คุณต้องมีสิทธิ์การใช้งานอย่างน้อยหนึ่งสิทธิ์ที่มอบหมายในองค์กรของคุณ
  - **ระบบคลาวด์เฉพาะผู้ใช้**- บัญชีOffice 365 (O365) ที่ชําระเงิน SKU หรือ Azure AD Basic
  - **ผู้ใช้ระบบคลาวด์และ/หรือภายในองค์กร**- Azure AD Premium P1 หรือ P2, Enterprise Mobility + Security (EMS) หรือ Secure Productive Enterprise (SPE)
    - เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับข้อกฎหมายด้านสิทธิ์การใช้งาน ให้ดู [ข้อกฎหมายเกี่ยวกับสิทธิ์การใช้งานในการตั้งค่ารหัสผ่านแบบบริการตนเองของ Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- คุณมีบัญชีผู้ดูแลระบบอย่างน้อยหนึ่งบัญชีและทดสอบบัญชีผู้ใช้หนึ่งบัญชีด้วยหนึ่งในสิทธิ์การใช้งานที่เหมาะสม
- คุณต้องเชื่อมต่อตัวระบุเชื่อมต่อ Azure AD กับตัว Emulator ตัวควบคุมโดเมนหลักเพื่อให้การเขียนกลับของรหัสผ่านสามารถได้ผล คุณสามารถกําหนดค่าตัวเชื่อมต่อ Azure AD เพื่อใช้ตัวควบคุมโดเมนหลักโดยคลิกขวาที่คุณสมบัติของตัวเชื่อมต่อการซิงโครไนซ์ Active  Directory แล้วเลือก **กําหนดค่าพาร์ติชัน** ไดเรกทอรี จากที่นั่น ให้ **ค้นหาส่วน การตั้งค่าการเชื่อมต่อ** ตัวควบคุมโดเมน และตรวจสอบกล่องที่ชื่อ **ใช้ตัวควบคุมโดเมนที่ต้องการ** เท่านั้น
    **หมายเหตุ**:ถ้า DC ที่ต้องการไม่ใช่ตัวเลียนแบบ PDC โปรแกรมเชื่อมต่อ Azure AD จะยังคงติดต่อ PDC เพื่อเขียนรหัสผ่าน
- การรีเซ็ตรหัสผ่านได้รับการกําหนดค่าและเปิดใช้งานในผู้เช่าของคุณแล้ว ดูข้อมูลเพิ่มเติมที่ [เปิดใช้งานผู้ใช้เพื่อรีเซ็ตรหัสผ่าน Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)ของพวกเขา
- ตรวจสอบให้แน่ใจว่าบัญชีผู้ดูแลระบบที่ใช้เพื่อเปิดใช้งาน Password Writeback เป็นบัญชีผู้ดูแลระบบระบบคลาวด์ (ที่สร้างใน Azure AD ไม่ใช่ AD ภายในองค์กร)
- คุณมีการปรับใช้ AD ภายในองค์กรแบบหลายฟอเรสต์เดียวหรือหลายฟอเรสต์ที่ใช้งาน Windows Server 2008 R2, Windows Server 2012 หรือ Windows Server 2012 R2 ที่มี Service Pack ล่าสุดติดตั้งอยู่
- คุณได้ติดตั้งเครื่องมือการเชื่อมต่อ Azure AD และคุณได้จัดเตรียมสภาพแวดล้อม AD ของคุณไว้เพื่อซิงโครไนซ์กับระบบคลาวด์ ก่อนที่จะทดสอบ Writeback ของรหัสผ่าน ตรวจสอบให้แน่ใจว่าคุณได้เสร็จสิ้นการนําเข้าและการซิงค์แบบเต็มจากทั้ง AD และ Azure AD เชื่อมต่อ Azure AD
- เมื่อต้องการเรียนรู้เพิ่มเติม ดูวิธีการซิงค์และ[นําเข้าแบบเต็มในบัญชีผู้ใช้ Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)เชื่อมต่อ

**ฉันมีปัญหากับการเชื่อมต่อ Writeback ของรหัสผ่าน**

1. ดาวน์โหลดและเปิดใช้งาน Azure AD เวอร์ชันล่าสุด[เชื่อมต่อ](https://www.microsoft.com/download/details.aspx?id=47594)
2. การกําหนดค่าไฟร์วอลล์: เชื่อมต่อ Azure AD (1.1.443 ขึ้นไป) ต้องการ **การเข้าถึง HTTPS** ขาออกเพื่อ:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. อนุญาตให้การเชื่อมต่อที่ไม่ได้ใช้งานยังคงอยู่เป็นเวลาอย่างน้อย 2-3 นาที

**ฉันยังคงมีปัญหากับการเขียนรหัสผ่าน**

- ถ้าคุณยังคงประสบปัญหา ลองปิดใช้งานและเปิดใช้งานบริการการเขียนกลับของรหัสผ่านอีกครั้งในเครื่องมือยืนยันรหัสผ่านของ Azure AD เชื่อมต่อ
- เมื่อต้องการเรียนรู้เพิ่มเติม ดูวิธีการ [ปิดใช้งานและเปิดใช้งานการเขียนรหัสผ่านอีกครั้ง](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
