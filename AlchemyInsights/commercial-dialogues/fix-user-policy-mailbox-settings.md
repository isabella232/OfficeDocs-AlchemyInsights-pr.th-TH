---
title: แก้ไขการตั้งค่านโยบาย/กล่องจดหมายของผู้ใช้
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034737"
---
# <a name="fix-user-policymailbox-settings"></a>แก้ไขการตั้งค่านโยบาย/กล่องจดหมายของผู้ใช้

การตั้งค่าอีเมลขยะบนกล่องจดหมายจะได้รับผลกระทบจากข้อความนี้ เมื่อต้องการรีวิวการตั้งค่า ให้ทต่อไปนี้:

1. เปิดใช้ Exchange Management Shell For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).
2. เรียกใช้การสั่งนี้ (โดยใช้ที่อยู่อีเมลของผู้ใช้):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. ตรวจสอบว่าที่อยู่อีเมลของผู้ส่งเป็นส่วนหนึ่งของ **TrustedSendersAndDomains** **หรือ BlockedSendersAndDomains** หรือไม่ ถ้าที่อยู่อีเมลอยู่ในรายการใดรายการหนึ่ง คุณอาจต้องเอาที่อยู่อีเมลออก เมื่อต้องการเรียนรู้เพิ่มเติม ให้ดู[Set-MailboxJunkAmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047)
