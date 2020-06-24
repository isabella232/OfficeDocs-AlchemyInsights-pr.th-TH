---
title: สิทธิ์ในปฏิทิน
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862165"
---
# <a name="calendar-permissions"></a>สิทธิ์ในปฏิทิน

ผู้ใช้สามารถเปลี่ยนสิทธิ์ในปฏิทินของตนเองกับ Outlook บนเว็บหรือไคลเอนต์อื่น ๆ แต่เป็นผู้ดูแลระบบคุณอาจต้องตรวจสอบเช่นกัน  
ด้วย cmdlet PowerShell อัตราแลกเปลี่ยนจะแสดงสิทธิ์บนปฏิทินของผู้ใช้:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

เมื่อต้องการดูข้อมูลเพิ่มเติม ให้ดูต่อไปนี้:

- [รับกล่องจดหมายโฟลเดอร์เปอร์mission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [ตั้งค่ากล่องจดหมายโฟลเดอร์เปอร์mission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [เพิ่มกล่องจดหมายโฟลเดอร์เปอร์mission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

สิทธิ์ในปฏิทินจะใช้ในการแชร์ปฏิทิน เพื่อดูข้อมูลเพิ่มเติมเกี่ยวกับการใช้ปฏิทิน Outlook ร่วมกัน ให้ดูบทความต่อไปนี้

- [แชร์ปฏิทิน Outlook กับบุคคลอื่น](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [แชร์ปฏิทินของคุณใน Outlook บนเว็บสําหรับธุรกิจ](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

เมื่อต้องการแก้ไขปัญหาสิทธิ์ในปฏิทิน คุณสามารถใช้เครื่องมือ['ตัวช่วยช่วยเหลือและการกู้คืน'](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)