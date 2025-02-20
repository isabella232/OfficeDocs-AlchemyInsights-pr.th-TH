---
title: นโยบายการเก็บข้อมูลใน Exchangeศูนย์การจัดการไม่ใช้งานได้
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 6652ad5fc1691e1d5a4293d81f3a649f23ec38f18c8ed9fe06665628a901d13e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074951"
---
# <a name="retention-policies-in-exchange-admin-center"></a>นโยบายการเก็บข้อมูลในExchangeการจัดการ

ถ้าคุณต้องการให้เราเรียกใช้การตรวจสอบการตั้งค่าที่กล่าวถึงด้านล่างโดยอัตโนมัติ ให้เลือกปุ่ม ย้อนกลับ < ที่ด้านบนของหน้านี้ จากนั้นใส่ที่อยู่อีเมลของผู้ใช้ที่มีปัญหากับนโยบายการเก็บข้อมูล

ถ้าคุณมีปัญหากับนโยบายการเก็บข้อมูลในศูนย์Exchangeกล่องจดหมายหรือรายการที่ไม่ได้ย้ายไปยังกล่องจดหมายเก็บถาวร ให้ตรวจสอบดังต่อไปนี้:

**สาเหตุหลัก:**

- **ตัวช่วยโฟลเดอร์ที่มี** การจัดการไม่ได้ประมวลผลกล่องจดหมายของผู้ใช้ ตัวช่วยโฟลเดอร์ที่มีการจัดการจะพยายามประมวลผลกล่องจดหมายทั้งหมดในองค์กรระบบคลาวด์ของคุณทุกๆ 7 วัน

  **วิธีแก้ไข:** เรียกใช้ตัวช่วยจัดการโฟลเดอร์

- **มีการเปิดใช้งาน RetentionHold** บนกล่องจดหมายแล้ว ถ้ากล่องจดหมายถูกวางไว้ใน RetentionHold นโยบายการเก็บข้อมูลบนกล่องจดหมายจะไม่ถูกประมวลผลระหว่างช่วงเวลาดังกล่าว

  **วิธีแก้ไข:** ตรวจสอบสถานะของการตั้งค่าการหยุดการเก็บข้อมูลและอัปเดตตามต้องการ For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**หมายเหตุ:** ถ้ากล่องจดหมายมีขนาดเล็กกว่า 10 MB ตัวช่วยจัดการโฟลเดอร์จะไม่ประมวลผลกล่องจดหมายโดยอัตโนมัติ
 
For more info on retention policies in the Exchange Admin Center, see:

- [แท็กการเก็บข้อมูลและนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [ใช้นโยบายการเก็บข้อมูลกับกล่องจดหมาย หรือเพิ่ม](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)[หรือเอาแท็กการเก็บข้อมูลออก](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [วิธีการระบุชนิดของการหยุดบนกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
