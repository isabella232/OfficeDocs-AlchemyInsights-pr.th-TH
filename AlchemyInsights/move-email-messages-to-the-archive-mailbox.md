---
title: ย้ายข้อความทาง e-mail ไปยังกล่องจดหมายเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822181"
---
# <a name="move-email-to-the-archive-mailbox"></a>ย้ายเมลไปยังกล่องจดหมายเก็บถาวร

1. ยืนยันว่า**กล่องจดหมายเก็บถาวร**ถูกเปิดใช้งาน ถ้าไม่ให้ใช้ขั้นตอนใน[บทความนี้](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)เพื่อเปิดใช้งานกล่องจดหมายเก็บถาวร

2. ในการเก็บถาวรข้อความไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติจะต้องตั้งค่าแท็กการเก็บข้อมูลที่มีการ**ย้ายไปยังการเก็บถาวร**การดำเนินการที่จะ**นำไปใช้โดยอัตโนมัติไปยังกล่องจดหมายทั้งหมด (เริ่มต้น)** ใช้ขั้นตอนที่นี่เพื่อสร้างแท็ก:[แท็กเริ่มต้นที่เก็บถาวร](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. จากนั้นให้เพิ่มแท็ก**เก็บถาวร**ในนโยบายการเก็บข้อมูลของคุณ ในศูนย์ดูแล Exchange เลือกนโยบายการ**เก็บข้อมูล**> เพิ่มการ**ย้ายไปยังแท็กเก็บถาวร**ไปยังนโยบาย >**บันทึก**

4. ตอนนี้[กำหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)ให้กับกล่องจดหมายของผู้ใช้ที่เฉพาะเจาะจง นโยบายเดียวกันจะถูกนำไปใช้กับทั้งกล่องจดหมาย**หลัก**และ**เก็บถาวร**

คุณอาจจำเป็นต้องบังคับให้มีการจัดการโฟลเดอร์ผู้ช่วย (MFA) เพื่อเรียกใช้และใช้การตั้งค่าใหม่กับกล่องจดหมายของตัวเอง เรียกใช้คำสั่งต่อไปนี้ในขณะที่[เชื่อมต่อกับ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)เพื่อเริ่มต้นผู้ช่วยโฟลเดอร์ที่มีการจัดการสำหรับกล่องจดหมายที่ระบุ:
  
ผู้ช่วยเริ่มต้นการจัดการ-เอกลักษณ์<name of the mailbox>

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวรโปรดดูที่[การตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมาย](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  