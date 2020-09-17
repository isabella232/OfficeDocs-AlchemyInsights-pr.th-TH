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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799799"
---
# <a name="move-email-to-the-archive-mailbox"></a>ย้ายอีเมลไปยังกล่องจดหมายเก็บถาวร

ถ้าคุณต้องการให้เราเรียกใช้การตรวจสอบโดยอัตโนมัติสำหรับการตั้งค่าที่ระบุไว้ด้านล่างให้เลือกปุ่มย้อนกลับ <-ที่ด้านบนสุดของหน้านี้แล้วใส่ที่อยู่อีเมลของผู้ใช้ที่มีปัญหาในการย้ายอีเมลไปยังกล่องจดหมายเก็บถาวรของพวกเขา

1. ยืนยันว่า **กล่องจดหมายเก็บถาวร** ถูกเปิดใช้งานแล้ว ถ้าไม่ใช่ให้ใช้ขั้นตอนใน [บทความนี้](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) เพื่อเปิดใช้งานกล่องจดหมายเก็บถาวร

2. เมื่อต้องการเก็บถาวรข้อความโดยอัตโนมัติไปยังกล่องจดหมายเก็บถาวรแท็กการเก็บข้อมูลที่มีการดำเนินการ**ย้ายไปยังการเก็บถาวร**ต้องถูกตั้งค่าให้**นำไปใช้โดยอัตโนมัติไปยังแท็กกล่องจดหมาย (ค่าเริ่มต้น) ทั้งหมด** ใช้ขั้นตอนต่อไปนี้เพื่อสร้างแท็ก:[แท็กเริ่มต้นของการเก็บถาวร](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)

3. ถัดไปให้เพิ่มแท็ก **เก็บถาวร** ลงในนโยบายการเก็บข้อมูลของคุณ ในศูนย์การจัดการ Exchange ให้เลือก**นโยบายการเก็บข้อมูล**> เพิ่ม**แท็กย้ายไปยังการเก็บถาวร**ในนโยบาย >**บันทึก**

4. ในตอนนี้ให้ [กำหนดนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) ให้กับกล่องจดหมายของผู้ใช้ที่ระบุ นโยบายเดียวกันจะถูกนำไปใช้กับทั้งกล่องจดหมาย**หลัก**และกล่องจดหมาย**เก็บถาวร**

คุณอาจจำเป็นต้องบังคับใช้ตัวช่วยสร้างโฟลเดอร์ที่มีการจัดการ (MFA) เพื่อเรียกใช้และนำการตั้งค่าใหม่ไปใช้กับกล่องจดหมายของผู้ใช้ เรียกใช้คำสั่งต่อไปนี้ในขณะ [ที่เชื่อมต่อกับ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) เพื่อเริ่มต้นตัวช่วยสร้างโฟลเดอร์ที่มีการจัดการสำหรับกล่องจดหมายที่เฉพาะเจาะจง:
  
เริ่มต้น-ManagedFolderAssistant-ข้อมูลประจำตัว <name of the mailbox>

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการตั้งค่านโยบายการเก็บถาวรให้ดู[ที่ตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  