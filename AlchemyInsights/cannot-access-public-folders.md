---
title: ไม่สามารถเข้าถึงโฟลเดอร์สาธารณะ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959513"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ไม่สามารถเชื่อมต่อไปยังโฟลเดอร์สาธารณะ

ถ้าการเข้าถึงโฟลเดอร์สาธารณะไม่ทำงานสำหรับผู้ใช้ไม่กี่ให้ลองทำดังต่อไปนี้:

เชื่อมต่อกับ EXO PowerShell และกำหนดค่าการ DefaultPublicFolderMailbox จดหมายบนบัญชีผู้ใช้ที่มีปัญหาเพื่อให้ตรงกับหนึ่งในบัญชีผู้ใช้ที่ทำงาน

ตัว อย่าง เช่น:

ได้รับกล่องจดหมายผู้ใช้ , EffectivePublicFolderMailbox

กล่องจดหมาย ProblemUser \<ค่าจากคำสั่งก่อนหน้านี้>

รออย่างน้อยหนึ่งชั่วโมงสำหรับการเปลี่ยนแปลงมีผลบังคับใช้