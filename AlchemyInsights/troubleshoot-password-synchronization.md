---
title: การแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732529"
---
# <a name="troubleshoot-password-synchronization"></a>การแก้ไขปัญหาการซิงโครไนส์รหัสผ่าน

เมื่อต้องการแก้ไขปัญหาที่ไม่มีรหัสผ่านจะซิงโครไนส์กับ Azure AD Connect รุ่น 1.1.614.0 หรือรุ่นที่ใหม่กว่า:
  
1. เปิดเซสชัน Windows PowerShell ใหม่บนเซิร์ฟเวอร์ Azure AD Connect ของคุณด้วย**การเรียกใช้ในฐานะผู้ดูแล**ตัวเลือก

2. เรียกใช้**ชุด ExecutionPolicy RemoteSigned**หรือ**ชุด ExecutionPolicy ไม่ จํากัด**

3. เริ่มตัวช่วยสร้างการเชื่อมต่อ AD Azure

4. นําทางไปยังหน้า**งานเพิ่มเติม****Troubleshoot****Next**

5. บนหน้า การแก้ไขปัญหา ให้คลิก**เปิดใช้ เพื่อเริ่มเมนูการแก้ไขปัญหา**ใน PowerShell

6. ในเมนูหลัก**ให้เลือก**

7. ในเมนูย่อย ให้เลือก**การซิงโครไนซ์รหัสผ่าน ไม่ทํางานเลย**

**ทําความเข้าใจผลลัพธ์ของงานการแก้ไขปัญหา**
  
งานการแก้ไขปัญหาทําการตรวจสอบต่อไปนี้:
  
- ตรวจสอบว่า เปิดใช้งานคุณลักษณะการซิงโครไนส์รหัสผ่านสําหรับผู้เช่า Azure AD ของคุณ

- ตรวจสอบว่า เซิร์ฟเวอร์เชื่อมต่อ AD Azure ไม่ได้อยู่ในโหมดการจัดเตรียม

- สําหรับแต่ละตัวเชื่อมต่อ Active Directory ที่มีอยู่ในสถานที่ (ซึ่งสอดคล้องกับฟอเรสต์ Active Directory ที่มีอยู่):

- 
  - ตรวจสอบว่าเปิดใช้งานคุณลักษณะการซิงโครไนส์รหัสผ่าน

  - ค้นหาเหตุการณ์ heartbeat ฮาร์ทบีทรหัสผ่านในบันทึกเหตุการณ์ของโปรแกรมประยุกต์ Windows

  - สําหรับแต่ละโดเมน Active Directory ภายใต้ตัวเชื่อมต่อ Active Directory ในสถาน:

  - ตรวจสอบว่า โดเมนสามารถเข้าถึงได้จากเซิร์ฟเวอร์การเชื่อมต่อ AD Azure

  - ตรวจสอบว่า บัญชีบริการระบบโดเมนไดเรกทอรีที่ใช้งานอยู่ (AD DS) ที่ใช้โดยตัวเชื่อมต่อ Active Directory ในสถานที่มีชื่อผู้ใช้ รหัสผ่าน และสิทธิ์ที่ถูกต้องที่จําเป็นสําหรับการซิงโครไนส์ของรหัสผ่าน

สําหรับความช่วยเหลือเพิ่มเติมในการแก้ไขปัญหาการซิงค์รหัสผ่าน ให้ดูที่[การแก้ไขปัญหาการซิงค์รหัสผ่านกับการซิงค์ Ad Connect ของ Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)
  