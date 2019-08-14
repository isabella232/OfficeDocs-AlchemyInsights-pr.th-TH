---
title: 305 เพิ่มขนาดกล่องจดหมายเก็บถาวร
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 28086145d8769bd06ef6352257a820146c5f237d
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: th-TH
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391585"
---
# <a name="increase-the-archive-mailbox-size"></a>เพิ่มขนาดกล่องจดหมายเก็บถาวร

Office 365[ขีดจำกัด](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits)ขนาดของกล่องจดหมายที่เก็บถาวรที่ขึ้นอยู่กับสิทธิ์การใช้งานที่ถูกกำหนดให้กับบัญชีผู้ใช้ เมื่อกล่องจดหมายเก็บถาวรถึง 90% ของขนาดที่ใช้ได้ ผู้ใช้ได้รับการแจ้งเตือนทางอีเมล เมื่อกล่องจดหมายการเก็บถาวรได้ถึงขีดจำกัดของขนาด ผู้ใช้ไม่สามารถย้ายรายการไปยังกล่องจดหมายการเก็บถาวร Office 365 จะไม่เพิ่มขนาดของกล่องจดหมายเก็บถาวรเมื่อถึงขนาดจำกัดไว้ แทน ผู้ใช้สามารถดำเนินการดังต่อไปนี้เพื่อเพิ่มเนื้อที่ในการเก็บถาวรกล่องจดหมาย:

- ส่งออกรายการไปยังแฟ้ม.pst โดยใช้ Outlook

- ลบรายการออกจากกล่องจดหมายเก็บถาวร

Office 365 ให้**เก็บถาวรไม่จำกัด**สำหรับใบอนุญาต E3 องค์กร 365 Office และ E5 Admin ต้องเปิดใช้งานคุณลักษณะนี้ก่อนที่เก็บกล่องจดหมายมาถึงขนาดสูงสุด เมื่อมีการใช้การเก็บถาวรไม่จำกัด ซึ่งอาจใช้เวลาถึง 30 วันก่อนช่องว่างถูกเพิ่มไปยังกล่องจดหมายการเก็บถาวร ดังนั้น เราขอแนะนำให้ ผู้ดูแลตรวจสอบเนื้อที่ว่างในการเก็บถาวรกล่องจดหมาย ซึ่งช่วยให้ผู้ใช้ใช้กล่องจดหมายการเก็บถาวรในขณะนั้นขยายต่อไป สำหรับข้อมูลเพิ่มเติม ดู[ภาพรวมของการเก็บถาวรใน Office 365 ไม่จำกัด](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving)และการ[เปิดใช้งานการเก็บถาวรได้ไม่จำกัดใน Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving)

สำหรับข้อมูลเพิ่มเติมเกี่ยวกับการเข้าถึงกล่องจดหมายเก็บถาวรจาก Outlook ดู[ความต้องการของ Outlook สำหรับการเข้าถึงรายการในเก็บถาวรอัตโนมัติถูกขยาย](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive) เมื่อต้องการกำหนดค่านโยบายการเก็บข้อมูลที่ย้ายรายการไปยังกล่องจดหมายเก็บถาวรโดยอัตโนมัติ ดู[การตั้งค่านโยบายการเก็บถาวรและการลบสำหรับกล่องจดหมายในองค์กรของคุณ Office 365](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)

**หมายเหตุ**: แฟ้มเก็บถาวรที่ขยายได้อัตโนมัติไม่ได้รับการสนับสนุนสำหรับกล่องจดหมายหลักบน Exchange 2010
