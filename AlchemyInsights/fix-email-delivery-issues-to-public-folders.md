---
title: แก้ไขปัญหาการนําส่งอีเมลไปให้กับโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716371"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>แก้ไขปัญหาการนําส่งอีเมลไปให้กับโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมาย

ถ้าผู้ส่งภายนอกไม่สามารถส่งข้อความไปยังโฟลเดอร์สาธารณะที่เปิดใช้งานจดหมายของคุณ และผู้ส่งได้รับข้อผิดพลาด:**ไม่พบ (550 5.4.1)** ตรวจสอบว่าโดเมนอีเมลสําหรับโฟลเดอร์สาธารณะถูกกําหนดค่าเป็นโดเมนรีเลย์ภายในแทนโดเมนที่มีสิทธิ์:

1. เปิด[ศูนย์การจัดการ Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)

2. ไปที่\>**โดเมนที่ยอมรับ****ขั้นตอนจดหมาย**ให้เลือกโดเมนที่ยอมรับ แล้วคลิก**แก้ไข**

3. ในเพจคุณสมบัติที่เปิดขึ้น**Authoritative****Internal relay****Save**

ถ้าผู้ส่งภายนอกได้รับข้อผิดพลาด**ที่คุณไม่มีสิทธิ์ (550 5.7.13)** เรียกใช้คําสั่งต่อไปนี้ใน[PowerShell แบบออนไลน์ของอัตราแลกเปลี่ยน](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)เพื่อดูสิทธิ์สําหรับผู้ใช้ที่ไม่ระบุชื่อในโฟลเดอร์สาธารณะ:

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`ตัวอย่างเช่น`Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.

เมื่อต้องการอนุญาตให้ผู้ใช้ภายนอกส่งอีเมลไปยังโฟลเดอร์นี้สาธารณะ ตัวอย่างเช่น`Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
