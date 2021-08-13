---
title: ย้ายข้อความอีเมลไปยังกล่องจดหมายเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974976"
---
# <a name="move-email-to-the-archive-mailbox"></a>ย้ายอีเมลไปยังกล่องจดหมายเก็บถาวร

ถ้าคุณต้องการให้เราเรียกใช้การตรวจสอบการตั้งค่าที่กล่าวถึงด้านล่างโดยอัตโนมัติ ให้เลือกปุ่ม ย้อนกลับ < ที่ด้านบนของหน้านี้ แล้วใส่ที่อยู่อีเมลของผู้ใช้ที่มีปัญหาในการย้ายอีเมลไปยังกล่องจดหมายเก็บถาวรของพวกเขา

1. ยืนยันว่าได้ **เปิดใช้งานกล่องจดหมาย** เก็บถาวรแล้ว ถ้าไม่ ให้ใช้ขั้นตอน [ในบทความนี้เพื่อ](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) เปิดใช้งานกล่องจดหมายเก็บถาวร

2. เมื่อต้องการเก็บข้อความถาวรโดยอัตโนมัติไปยังกล่องจดหมายเก็บถาวร แท็กการเก็บข้อมูลที่มีการตั้งค่าการแอคชัน ย้ายไปยังการเก็บถาวร จะต้องตั้งค่าให้ใช้กับแท็ก กล่องจดหมายทั้งหมด **(ค่าเริ่มต้น)** โดยอัตโนมัติ ใช้ขั้นตอนที่นี่เพื่อสร้างแท็ก: แท็ก [เก็บถาวร](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)เริ่มต้น

3. ถัดไป ให้เพิ่ม **แท็ก** เก็บถาวร ลงในนโยบายการเก็บข้อมูล In the Exchange admin center, choose **Retention Policies** > the Move to **Archive tag** to the policy > **Save**.

4. [ในตอนนี้ ให้กําหนด](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)นโยบายการเก็บข้อมูลให้กับกล่องจดหมายของผู้ใช้ที่ระบุ นโยบายเดียวกันนี้จะถูกปรับใช้กับทั้ง **กล่องจดหมาย** หลักและ **กล่องจดหมาย** เก็บถาวร

อาจจําเป็นต้องบังคับให้ตัวช่วยโฟลเดอร์ที่มีการจัดการ (MFA) เรียกใช้และปรับใช้การตั้งค่าใหม่กับกล่องจดหมายของผู้ใช้ เรียกใช้สั่งต่อไปนี้ [ขณะเชื่อมต่อกับ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) เพื่อเริ่มตัวช่วยจัดการโฟลเดอร์ของกล่องจดหมายที่ระบุ:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

For more information on setting up an archive policy, [see Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  