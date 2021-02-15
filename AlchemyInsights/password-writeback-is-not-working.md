---
title: Password Writeback ไม่ใช้งาน
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
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243525"
---
# <a name="password-writeback-is-not-working"></a>Password Writeback ไม่ใช้งาน

**ฉันมีปัญหาในการกําหนดค่า Writeback ของรหัสผ่าน**

- Password Writeback เป็นฟีเจอร์ระดับพรีเมียม
- ตรวจสอบให้แน่ใจว่าคุณเข้าใจความต้องการด้านสิทธิ์การใช้งาน:
  - คุณต้องมีอย่างน้อยหนึ่งสิทธิ์การใช้งานที่มอบหมายในองค์กรของคุณ
  - **ระบบคลาวด์เฉพาะผู้ใช้** - Office 365 (O365) ชําระเงิน SKU หรือ Azure AD Basic
  - **ผู้ใช้ระบบคลาวด์และ/หรือผู้ใช้ในองค์กร** - Azure AD Premium P1 หรือ P2, Enterprise Mobility + Security (EMS) หรือ Secure Productive Enterprise (SPE)
    - เมื่อต้องการเรียนรู้เพิ่มเติมเกี่ยวกับข้อตามความต้องการด้านสิทธิ์การใช้งาน ให้ดู [ข้อกฎหมายการให้สิทธิ์การใช้งานรีเซ็ตรหัสผ่านด้วยตนเองของ Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- คุณมีบัญชีผู้ดูแลระบบอย่างน้อยหนึ่งบัญชีและบัญชีผู้ใช้ทดสอบหนึ่งบัญชีที่มีหนึ่งในสิทธิ์การใช้งานที่เหมาะสม
- คุณต้องเชื่อมต่อ Azure AD Connect กับตัว Emulator ของตัวควบคุมโดเมนหลักเพื่อให้สามารถใช้งานการเขียนรหัสผ่านได้ คุณสามารถกําหนดค่า Azure AD Connect ให้ใช้ตัวควบคุมโดเมนหลักโดยคลิกขวาที่คุณสมบัติของตัวเชื่อมต่อการซิงโครไนซ์ Active Directory แล้วเลือก **กําหนดค่าพาร์ติชัน** ไดเรกทอรี จากที่นั่น ให้ค้นหา **ส่วนการตั้งค่าการเชื่อมต่อ** ตัวควบคุมโดเมน และตรวจสอบกล่องที่มีชื่อเรื่อง **ว่าใช้ตัวควบคุมโดเมนที่ต้องการ** เท่านั้น
  > [!NOTE]
  > ถ้า DC ที่ต้องการไม่ใช่ตัวเลียนแบบ PDC Azure AD Connect จะยังคงติดต่อไปยัง PDC เพื่อเขียนรหัสผ่าน
- การกําหนดค่าและเปิดใช้งานการตั้งค่ารหัสผ่านใหม่ในผู้เช่าของคุณ หากต้องการข้อมูลเพิ่มเติม โปรดดู [การเปิดใช้งานผู้ใช้เพื่อตั้งค่ารหัสผ่าน Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)ใหม่
- ตรวจสอบให้แน่ใจว่าบัญชีผู้ดูแลระบบที่ใช้เพื่อเปิดใช้งาน Password Writeback เป็นบัญชีผู้ดูแลระบบระบบคลาวด์ (ที่สร้างใน Azure AD ไม่ใช่ AD ภายในองค์กร)
- คุณมีการปรับใช้แบบภายในองค์กรแบบหลายฟอเรสต์หรือหลายฟอเรสต์ที่ใช้งาน Windows Server 2008 R2, Windows Server 2012 หรือ Windows Server 2012 R2 ที่มี Service Pack ล่าสุดติดตั้งอยู่
- คุณได้ติดตั้งเครื่องมือ Azure AD Connect และได้จัดเตรียมสภาพแวดล้อม AD ของคุณไว้เพื่อซิงโครไนซ์กับระบบคลาวด์ ก่อนที่จะทดสอบ Writeback ของรหัสผ่าน ตรวจสอบให้แน่ใจว่าคุณเสร็จสิ้นการนําเข้าและการซิงค์แบบเต็มจากทั้ง AD และ Azure AD ใน Azure AD Connect
- เมื่อต้องการเรียนรู้เพิ่มเติม ดูวิธีการซิงค์แบบเต็ม [และนําเข้าแบบเต็มใน Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**ฉันมีปัญหากับการเชื่อมต่อ Writeback ของรหัสผ่าน**

1. ดาวน์โหลดและเปิดใช้งาน [Azure AD Connect เวอร์ชันล่าสุด](https://www.microsoft.com/download/details.aspx?id=47594)
2. การกําหนดค่าไฟร์วอลล์: เครื่องมือ Azure AD Connect (1.1.443 ขึ้นไป) จะต้อง **มีสิทธิ์การเข้าถึง HTTPS** ขาออก:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. อนุญาตให้การเชื่อมต่อที่ไม่ได้ใช้งานยังคงอยู่เป็นเวลาอย่างน้อย 2-3 นาที

**ฉันยังคงมีปัญหากับ Writeback รหัสผ่าน**

- ถ้าคุณยังพบปัญหา ให้ลองปิดใช้งานและเปิดใช้งานบริการ Writeback ของรหัสผ่านอีกครั้งในเครื่องมือ Azure AD Connect
- เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดูวิธีการปิดใช้งาน [และเปิดใช้งาน Writeback รหัสผ่านอีกครั้ง](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
