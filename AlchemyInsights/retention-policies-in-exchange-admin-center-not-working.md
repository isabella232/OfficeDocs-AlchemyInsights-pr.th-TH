---
title: นโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange ไม่ใช้งาน
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952247"
---
# <a name="retention-policies-in-exchange-admin-center"></a>นโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange

ถ้าคุณต้องการให้เราเรียกใช้การตรวจสอบการตั้งค่าที่กล่าวถึงด้านล่างโดยอัตโนมัติ ให้เลือกปุ่ม ย้อนกลับ < ที่ด้านบนของหน้านี้ จากนั้นใส่ที่อยู่อีเมลของผู้ใช้ที่มีปัญหากับนโยบายการเก็บข้อมูล

ถ้าคุณมีปัญหากับนโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange จะไม่ใช้กับกล่องจดหมายหรือรายการที่ไม่ได้ย้ายไปยังกล่องจดหมายเก็บถาวร ให้ตรวจสอบดังต่อไปนี้:

**สาเหตุหลัก:**

- **ตัวช่วยโฟลเดอร์ที่มี** การจัดการไม่ได้ประมวลผลกล่องจดหมายของผู้ใช้ ตัวช่วยโฟลเดอร์ที่มีการจัดการจะพยายามประมวลผลกล่องจดหมายทั้งหมดในองค์กรระบบคลาวด์ของคุณทุกๆ 7 วัน

  **วิธีแก้ไข:** เรียกใช้ตัวช่วยจัดการโฟลเดอร์

- **มีการเปิดใช้งาน RetentionHold** บนกล่องจดหมายแล้ว ถ้ากล่องจดหมายถูกวางไว้ใน RetentionHold นโยบายการเก็บข้อมูลบนกล่องจดหมายจะไม่ถูกประมวลผลระหว่างช่วงเวลาดังกล่าว

  **วิธีแก้ไข:** ตรวจสอบสถานะของการตั้งค่าการหยุดการเก็บข้อมูลและอัปเดตตามต้องการ For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
 
**หมายเหตุ:** ถ้ากล่องจดหมายมีขนาดเล็กกว่า 10 MB ตัวช่วยจัดการโฟลเดอร์จะไม่ประมวลผลกล่องจดหมายโดยอัตโนมัติ
 
ดูข้อมูลเพิ่มเติมเกี่ยวกับนโยบายการเก็บข้อมูลในศูนย์การจัดการ Exchange ที่:

- [แท็กการเก็บข้อมูลและนโยบายการเก็บข้อมูล](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- [ใช้นโยบายการเก็บข้อมูลกับกล่องจดหมาย หรือเพิ่ม](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)[หรือเอาแท็กการเก็บข้อมูลออก](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)

- [วิธีการระบุชนิดของการหยุดบนกล่องจดหมาย](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
