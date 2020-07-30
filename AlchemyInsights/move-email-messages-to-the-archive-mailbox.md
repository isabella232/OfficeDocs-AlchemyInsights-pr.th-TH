---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายการเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522790"
---
# <a name="move-email-to-the-archive-mailbox"></a>ย้ายอีเมลไปยังกล่องจดหมายเก็บถาวร

หากคุณต้องการให้เราเรียกใช้การตรวจสอบอัตโนมัติสําหรับการตั้งค่าที่กล่าวถึงด้านล่างให้เลือกปุ่มย้อนกลับ< -- ที่ด้านบนของหน้านี้แล้วป้อนที่อยู่อีเมลของผู้ใช้ที่มีปัญหาในการย้ายอีเมลไปยังกล่องจดหมายที่เก็บถาวรของพวกเขา

1. ยืนยันว่า**กล่องจดหมายเก็บถาวร**ถูกเปิดใช้งาน ถ้าไม่ใช่ ให้ใช้ขั้นตอน[ในบทความนี้](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)เพื่อเปิดใช้งานกล่องจดหมายเก็บถาวร

2. เมื่อต้องการเก็บถาวรข้อความไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ**Move to archive****applied automatically to entire mailbox (default) tag** ใช้ขั้นตอนในการสร้างแท็ก:[เก็บแท็กเริ่มต้นเก็บถาวร](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. จากนั้นให้เพิ่มแท็ก**เก็บถาวร**ลงในนโยบายการเก็บข้อมูล ในศูนย์การจัดการ Exchange เลือก**นโยบายการเก็บข้อมูล**>เพิ่ม**แท็กย้ายไปยังเก็บถาวร**นโยบาย>**บันทึก**

4. ตอนนี้[กําหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)ให้กับกล่องจดหมายของผู้ใช้ที่ระบุ นโยบายเดียวกันจะถูกนําไปใช้กับกล่องจดหมาย**หลัก**และการ**เก็บถาวร**

อาจจําเป็นต้องบังคับโฟลเดอร์ที่มีการจัดการช่วย (MFA) เพื่อเรียกใช้ และใช้การตั้งค่าใหม่ไปยังกล่องจดหมายของผู้ใช้ เรียกใช้คําสั่งต่อไปนี้ในขณะที่เชื่อมต่อกับ[EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)เพื่อเริ่มต้นผู้ช่วยโฟลเดอร์ที่มีการจัดการสําหรับกล่องจดหมายที่ระบุ:
  
เริ่มต้นจัดการFolderAssistant -เอกลักษณ์<name of the mailbox>

สําหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวร ให้ดูที่[การตั้งค่านโยบายการเก็บถาวรและการลบสําหรับกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  